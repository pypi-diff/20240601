# Comparing `tmp/jobquery-0.0.1.tar.gz` & `tmp/jobquery-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobquery-0.0.1.tar", last modified: Fri May 31 15:13:48 2024, max compression
+gzip compressed data, was "jobquery-1.0.1.tar", last modified: Sat Jun  1 11:25:09 2024, max compression
```

## Comparing `jobquery-0.0.1.tar` & `jobquery-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 15:13:48.375477 jobquery-0.0.1/
--rw-rw-rw-   0        0        0      206 2024-05-31 15:13:48.374476 jobquery-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 15:13:48.355044 jobquery-0.0.1/jobQuery/
--rw-rw-rw-   0        0        0        0 2024-05-29 08:44:01.000000 jobquery-0.0.1/jobQuery/__init__.py
--rw-rw-rw-   0        0        0    27873 2024-05-31 14:27:30.000000 jobquery-0.0.1/jobQuery/jobAPI.py
-drwxrwxrwx   0        0        0        0 2024-05-31 15:13:48.373468 jobquery-0.0.1/jobQuery.egg-info/
--rw-rw-rw-   0        0        0      206 2024-05-31 15:13:48.000000 jobquery-0.0.1/jobQuery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-31 15:13:48.000000 jobquery-0.0.1/jobQuery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 15:13:48.000000 jobquery-0.0.1/jobQuery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 15:13:48.000000 jobquery-0.0.1/jobQuery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 15:13:48.375477 jobquery-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      587 2024-05-31 15:13:08.000000 jobquery-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:25:09.044171 jobquery-1.0.1/
+-rw-rw-rw-   0        0        0      206 2024-06-01 11:25:09.043177 jobquery-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 11:25:09.021904 jobquery-1.0.1/jobQuery/
+-rw-rw-rw-   0        0        0        0 2024-05-29 08:44:01.000000 jobquery-1.0.1/jobQuery/__init__.py
+-rw-rw-rw-   0        0        0    33090 2024-06-01 11:18:58.000000 jobquery-1.0.1/jobQuery/jobAPI.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:25:09.042170 jobquery-1.0.1/jobQuery.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 11:25:08.000000 jobquery-1.0.1/jobQuery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:25:09.044171 jobquery-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      587 2024-06-01 11:24:44.000000 jobquery-1.0.1/setup.py
```

### Comparing `jobquery-0.0.1/jobQuery/jobAPI.py` & `jobquery-1.0.1/jobQuery/jobAPI.py`

 * *Files 19% similar despite different names*

```diff
@@ -320,20 +320,20 @@
                 return jobs
             except mysql.connector.Error as e:
                 print("Error retrieving data from MySQL:", e)
         else:
             print("Connection to MySQL not established.")
 
     # filter 找出所有工作
-    def get_jobs_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF):
+    def get_jobs_id_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF, limit=None):
         if self.conn is not None:
             try:
                 cursor = self.conn.cursor()
                 query = '''
-                    SELECT * FROM job
+                    SELECT `job_id` FROM job
                     WHERE 1=1
                 '''
                 params = []
 
                 if category:
                     if isinstance(category, list):
                         query += '''AND job_id IN (
@@ -443,20 +443,23 @@
                 if days is not None:
                     query += ' AND update_time >= DATE_SUB(CURDATE(), INTERVAL %s DAY)'
                     params.append(days)
 
                 if min_salary is not None and max_salary is not None and max_salary >= min_salary:
                     query += 'AND salary_min BETWEEN %s AND %s OR salary_max BETWEEN %s AND %s'
                     params.extend((min_salary, max_salary)*2)
+                
+                if limit is not None:
+                    query += ' LIMIT %s'
+                    params.append(limit)
 
                 cursor.execute(query, tuple(params))
                 jobs = cursor.fetchall()
 
                 return jobs
-
             except mysql.connector.Error as e:
                 print("Error retrieving data from MySQL:", e)
         else:
             print("Connection to MySQL not established.")
     
     def get_jobInfo_by_id(self, job_id):
         if job_id is 0 or job_id is None:
@@ -539,39 +542,156 @@
         else:
             print("Connection to MySQL not established.")
 
     def get_jobInfo(self, n):
         for i in range(n):
             yield self.get_jobInfo_by_id(i+1)
     
-    def get_jobInfo_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF):
-        jobs = self.get_jobs_by_filter(category=category,
-                                        skill=skill,
-                                        education=education,
-                                        tool=tool,
-                                        experience=experience,
-                                        days=days,
-                                        min_salary=min_salary,
-                                        max_salary=max_salary
-                                      )
-        # print(jobs)
-        for job in jobs:
-            # print(self.get_jobInfo_by_id(job[0]))
-            yield self.get_jobInfo_by_id(job[0])
+    def get_jobInfo_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF, limit=None):
+        if self.conn is not None:
+            try:
+                cursor = self.conn.cursor()
+                # 使用left join
+                # todo
+                
+            except mysql.connector.Error as e:
+                print("Error retrieving data from MySQL:", e)
     
     def get_number_by_filter(self, category=None, skill=None, education=None, tool=None, experience=None, days=None, min_salary=0, max_salary=INF):
-        return len(self.get_jobs_by_filter(category=category,
-                                        skill=skill,
-                                        education=education,
-                                        tool=tool,
-                                        experience=experience,
-                                        days=days,
-                                        min_salary=min_salary,
-                                        max_salary=max_salary
-                                      ))
+        if self.conn is not None:
+            try:
+                cursor = self.conn.cursor()
+                query = '''
+                    SELECT COUNT(*) FROM job
+                    WHERE 1=1
+                '''
+                params = []
+
+                if category:
+                    if isinstance(category, list):
+                        query += '''AND job_id IN (
+                                        SELECT job_id FROM Job_Category
+                                        WHERE category_id IN (
+                                            SELECT category_id FROM Categories
+                                            WHERE category_name IN (
+                        '''
+                        query += ', '.join(['%s']*len(category))
+                        query += ')))'
+                        params.extend(category)
+                    else:
+                        query += '''
+                            AND job_id IN (
+                                SELECT job_id FROM Job_Category
+                                WHERE category_id IN (
+                                    SELECT category_id FROM Categories
+                                    WHERE category_name = %s
+                                )
+                            )
+                        '''
+                        params.append(category)
+
+                if skill:
+                    if isinstance(skill, list):
+                        query += '''AND job_id IN (
+                                        SELECT job_id FROM Job_Skill
+                                        WHERE skill_id IN (
+                                            SELECT skill_id FROM Skills
+                                            WHERE name IN (
+                        '''
+                        query += ', '.join(['%s']*len(skill))
+                        query += ')))'
+                        params.extend(skill)
+                    else:
+                        query += '''
+                            AND job_id IN (
+                                SELECT job_id FROM Job_Skill
+                                WHERE skill_id IN (
+                                    SELECT skill_id FROM Skills
+                                    WHERE name = %s
+                                )
+                            )
+                        '''
+                        params.append(skill)
+
+                if experience:
+                    query += '''
+                        AND job_id IN (
+                            SELECT job_id FROM Job_Experience
+                            WHERE experience_id IN (
+                                SELECT experience_id FROM Experience
+                                WHERE experience = %s
+                            )
+                        )
+                    '''
+                    params.append(experience)
+
+                if education:
+                    if isinstance(education, list):
+                        query += '''
+                            AND job_id IN (
+                                SELECT job_id FROM Job_Education
+                                WHERE education_id IN (
+                                    SELECT education_id FROM Education
+                                    WHERE level IN (
+                        '''
+                        query += ', '.join(['%s']*len(education))
+                        query += ')))'
+                        params.extend(education)
+                    else:
+                        query += '''
+                            AND job_id IN (
+                                SELECT job_id FROM Job_Education
+                                WHERE education_id IN (
+                                    SELECT education_id FROM Education
+                                    WHERE level = %s
+                                )
+                            )
+                        '''
+                        params.append(education)
+
+                if tool:
+                    if isinstance(tool, list):
+                        query += '''
+                            AND job_id IN (
+                                SELECT job_id FROM Job_Tool
+                                WHERE tool_id IN (
+                                    SELECT tool_id FROM Tools
+                                    WHERE specialty_tool IN (
+                        '''
+                        query += ', '.join(['%s']*len(tool))
+                        query += ')))'
+                        params.extend(tool)
+                    else:
+                        query += '''
+                            AND job_id IN (
+                                SELECT job_id FROM Job_Tool
+                                WHERE tool_id IN (
+                                    SELECT tool_id FROM Tools
+                                    WHERE specialty_tool = %s
+                                )
+                            )
+                        '''
+                        params.append(tool)
+                
+                if days is not None:
+                    query += ' AND update_time >= DATE_SUB(CURDATE(), INTERVAL %s DAY)'
+                    params.append(days)
+
+                if min_salary is not None and max_salary is not None and max_salary >= min_salary:
+                    query += 'AND salary_min BETWEEN %s AND %s OR salary_max BETWEEN %s AND %s'
+                    params.extend((min_salary, max_salary)*2)
+
+                cursor.execute(query, tuple(params))
+                jobs = cursor.fetchone()
+
+                return jobs[0]
+            except mysql.connector.Error as e:
+                print("Error retrieving data from MySQL:", e)
+        else:
+            print("Connection to MySQL not established.")
 
     def move_data_from(self, database):
         if self.conn is not None:
             try:
                 cursor = self.conn.cursor()
                 tables = self.get_all_table()
 
@@ -642,38 +762,40 @@
 # 測試連接與獲取資料
 def main():
     import pprint
     db = JobDatabase(
         host="localhost",
         username="root",
         password="9879",
-        database="job104"
+        database="jobDatabase"
     )
 
     print('=============================================')
     print(db.get_number_by_filter(category=None,
                                  skill=None,
                                  education=None,
                                  tool=['python'],
                                  experience=None,
                                  days=None,
                                  min_salary=None,
                                  max_salary=None))
 
-    jobs = db.get_jobInfo_by_filter(category=['後端工程師', '網路管理工程師'],
-                                 skill=None,
-                                 education=None,
-                                 tool=None,
-                                 experience=None,
-                                 days=None,
-                                 min_salary=None,
-                                 max_salary=None
-                                )
+    # jobs = db.get_jobInfo_by_filter(category=['後端工程師', '網路管理工程師'],
+    #                              skill=None,
+    #                              education=None,
+    #                              tool=None,
+    #                              experience=None,
+    #                              days=None,
+    #                              min_salary=None,
+    #                              max_salary=None
+    #                             )
     
-    name = 'jobs'
-    with open(fr'{name}.txt', 'w') as f:
-        data = [j for j in jobs]
-        pprint.pprint(data, stream=f)
+    # for i in jobs:
+    #     print(i)
+    # name = 'jobs'
+    # with open(fr'{name}.txt', 'w', encoding='utf-8') as f:
+    #     data = [j for j in jobs]
+    #     pprint.pprint(data, stream=f)
     #     pprint.pprint(data, stream=f)
 
 if __name__ == "__main__":
     main()
```

### Comparing `jobquery-0.0.1/setup.py` & `jobquery-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from setuptools import setup, find_packages
 setup(name='jobQuery',
-      version='0.0.1',
+      version='1.0.1',
       description='birds atttributes and functions',
       author='megnet',
       author_email='2290906844@qq.com',
       requires= ['numpy','matplotlib'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

