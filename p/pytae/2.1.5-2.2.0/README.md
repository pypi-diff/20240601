# Comparing `tmp/pytae-2.1.5.tar.gz` & `tmp/pytae-2.2.0.tar.gz`

## Comparing `pytae-2.1.5.tar` & `pytae-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pytae-2.1.5/requirements.txt
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pytae-2.1.5/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytae-2.1.5/.ipynb_checkpoints/LICENSE-checkpoint
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pytae-2.1.5/.ipynb_checkpoints/README-checkpoint.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pytae-2.1.5/.ipynb_checkpoints/pyproject-checkpoint.toml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pytae-2.1.5/.ipynb_checkpoints/requirements-checkpoint.txt
--rw-r--r--   0        0        0    64965 2020-02-02 00:00:00.000000 pytae-2.1.5/src/other_examples.ipynb
--rw-r--r--   0        0        0    23584 2020-02-02 00:00:00.000000 pytae-2.1.5/src/recon.ipynb
--rw-r--r--   0        0        0    64965 2020-02-02 00:00:00.000000 pytae-2.1.5/src/.ipynb_checkpoints/other_examples-checkpoint.ipynb
--rw-r--r--   0        0        0    23584 2020-02-02 00:00:00.000000 pytae-2.1.5/src/.ipynb_checkpoints/recon-checkpoint.ipynb
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/__init__.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/extend_pandas.py
--rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/general_utils.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/reconciller.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/.ipynb_checkpoints/extend_pandas-checkpoint.py
--rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/.ipynb_checkpoints/general_utils-checkpoint.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 pytae-2.1.5/src/pytae/.ipynb_checkpoints/reconciller-checkpoint.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pytae-2.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytae-2.1.5/LICENSE
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pytae-2.1.5/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pytae-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pytae-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pytae-2.2.0/requirements.txt
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pytae-2.2.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytae-2.2.0/.ipynb_checkpoints/LICENSE-checkpoint
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pytae-2.2.0/.ipynb_checkpoints/README-checkpoint.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pytae-2.2.0/.ipynb_checkpoints/pyproject-checkpoint.toml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pytae-2.2.0/.ipynb_checkpoints/requirements-checkpoint.txt
+-rw-r--r--   0        0        0    70569 2020-02-02 00:00:00.000000 pytae-2.2.0/src/other_examples.ipynb
+-rw-r--r--   0        0        0    23851 2020-02-02 00:00:00.000000 pytae-2.2.0/src/recon.ipynb
+-rw-r--r--   0        0        0    67926 2020-02-02 00:00:00.000000 pytae-2.2.0/src/.ipynb_checkpoints/other_examples-checkpoint.ipynb
+-rw-r--r--   0        0        0    23584 2020-02-02 00:00:00.000000 pytae-2.2.0/src/.ipynb_checkpoints/recon-checkpoint.ipynb
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/__init__.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/extend_pandas.py
+-rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/general_utils.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/reconciller.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/.ipynb_checkpoints/extend_pandas-checkpoint.py
+-rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/.ipynb_checkpoints/general_utils-checkpoint.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 pytae-2.2.0/src/pytae/.ipynb_checkpoints/reconciller-checkpoint.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pytae-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytae-2.2.0/LICENSE
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pytae-2.2.0/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pytae-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pytae-2.2.0/PKG-INFO
```

### Comparing `pytae-2.1.5/.github/workflows/publish-to-test-pypi.yml` & `pytae-2.2.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/.ipynb_checkpoints/LICENSE-checkpoint` & `pytae-2.2.0/.ipynb_checkpoints/LICENSE-checkpoint`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/.ipynb_checkpoints/pyproject-checkpoint.toml` & `pytae-2.2.0/.ipynb_checkpoints/pyproject-checkpoint.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytae"
-version = "2.1.5"
+version = "2.2.0"
 authors = [
   { name="Madhukar Kumar Jha", email="madhukar.k.jha@gmail.com" },
 ]
 description = "A package to enhance common day to day tasks in the life of a data scientist"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pytae-2.1.5/src/other_examples.ipynb` & `pytae-2.2.0/src/.ipynb_checkpoints/other_examples-checkpoint.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920395359848485%*

 * *Differences: {"'cells'": "{17: {'execution_count': 18, 'outputs': {1: {'execution_count': 18}, insert: [(0, "*

 * *            "OrderedDict([('name', 'stdout'), ('output_type', 'stream'), ('text', ['pivot_table is "*

 * *            "used with sum as agg because Index contains duplicate entries.\\n'])]))]}}, 18: "*

 * *            "{'execution_count': 19, 'outputs': {0: {'execution_count': 19}}}, 19: "*

 * *            "{'execution_count': 35, 'outputs': {0: {'execution_count': 35}}}, 21: {'id': "*

 * *            "'978a8e44-0b77-417e-bef3-988d […]*

```diff
@@ -1105,19 +1105,26 @@
             "source": [
                 "penguins.long(col='features',\n",
                 "              value='value').wide(col='features',aggfunc='sum').long(col='features',value='value').value.sum()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "id": "9639866f-2f66-4f4e-aac7-e010649e4956",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "pivot_table is used with sum as agg because Index contains duplicate entries.\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -1474,27 +1481,27 @@
                             "22                NaN  \n",
                             "23                NaN  \n",
                             "24                NaN  \n",
                             "25                NaN  \n",
                             "26                NaN  "
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "penguins.long(col='features',\n",
                 "              value='value').wide(col='features')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 19,
             "id": "692ba49c-0d78-41d6-aad7-fa8045503ed7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1574,15 +1581,15 @@
                             "1  one   B    2   y\n",
                             "2  one   C    3   z\n",
                             "3  two   A    4   q\n",
                             "4  two   B    5   w\n",
                             "5  two   C    6   t"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = pd.DataFrame({'foo': ['one', 'one', 'one', 'two', 'two',\n",
                 "                           'two'],\n",
@@ -1590,15 +1597,15 @@
                 "                   'baz': [1, 2, 3, 4, 5, 6],\n",
                 "                   'zoo': ['x', 'y', 'z', 'q', 'w', 't']})\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 35,
             "id": "6502a2f3-0751-4d89-b400-74e99a635f18",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1685,27 +1692,106 @@
                             "1  one   y  NaN  2.0  NaN\n",
                             "2  one   z  NaN  NaN  3.0\n",
                             "3  two   q  4.0  NaN  NaN\n",
                             "4  two   t  NaN  NaN  6.0\n",
                             "5  two   w  NaN  5.0  NaN"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 35,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.wide(col='bar', value='baz')"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 44,
+            "id": "bc07e66a-a207-48aa-8d66-d23656fb4d21",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>type</th>\n",
+                            "      <th>mean_bill_length_cm</th>\n",
+                            "      <th>mean_body_mass_g</th>\n",
+                            "      <th>count</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>Gentoo</td>\n",
+                            "      <td>4.750488</td>\n",
+                            "      <td>5076.016260</td>\n",
+                            "      <td>124</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>Adelie</td>\n",
+                            "      <td>3.897500</td>\n",
+                            "      <td>3709.659091</td>\n",
+                            "      <td>44</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "     type  mean_bill_length_cm  mean_body_mass_g  count\n",
+                            "1  Gentoo             4.750488       5076.016260    124\n",
+                            "0  Adelie             3.897500       3709.659091     44"
+                        ]
+                    },
+                    "execution_count": 44,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "(penguins\n",
+                ".query(\"island == 'Biscoe'\")                                          #dplyr filter\n",
+                ".filter(items=['species', 'island', 'bill_length_mm', 'body_mass_g']) #dplyr select \n",
+                ".assign(bill_length_cm=lambda x: x.bill_length_mm / 10)               #dplyr mutate\n",
+                ".groupby(['species', 'island'])                                       #dplyr groupby\n",
+                ".agg(mean_bill_length_cm=('bill_length_cm', 'mean'),                  #dplyr summarize\n",
+                "     mean_body_mass_g=('body_mass_g', 'mean'),\n",
+                "     count=('species', 'size'))\n",
+                ".reset_index()                                                        #dplyr ungroup\n",
+                ".sort_values('mean_body_mass_g', ascending=False)                     #dplyr arrange\n",
+                ".drop(columns=['island'])                                             #dplyr select\n",
+                ".rename(columns={'species':'type'})                                   #dplyr rename\n",
+                ")\n"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": null,
-            "id": "a3c398fa-5ad4-48d6-8b9d-a3cbd173706d",
+            "id": "978a8e44-0b77-417e-bef3-988d1178d85f",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `pytae-2.1.5/src/recon.ipynb` & `pytae-2.2.0/src/.ipynb_checkpoints/recon-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/src/.ipynb_checkpoints/other_examples-checkpoint.ipynb` & `pytae-2.2.0/src/other_examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991546669934379%*

 * *Differences: {"'cells'": "{14: {'outputs': {0: {'data': {'text/html': {insert: [(22, '      "*

 * *            "<th>bill_length_mm_sum</th>\\n'), (23, '      <th>bill_depth_mm_sum</th>\\n'), (24, "*

 * *            "'      <th>flipper_length_mm_sum</th>\\n'), (25, '      "*

 * *            "<th>body_mass_g_sum</th>\\n'), (35, '      <td>821.9</td>\\n'), (36, '      "*

 * *            "<td>389.5</td>\\n'), (37, '      <td>4118.0</td>\\n'), (38, '      "*

 * *            "<td>74125.0</td>\\n'), (46, '      <td>893.0</td>\\n'), (47, '      "*

 * *      […]*

```diff
@@ -960,112 +960,168 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>species</th>\n",
                             "      <th>island</th>\n",
                             "      <th>sex</th>\n",
                             "      <th>n</th>\n",
+                            "      <th>bill_length_mm_sum</th>\n",
+                            "      <th>bill_depth_mm_sum</th>\n",
+                            "      <th>flipper_length_mm_sum</th>\n",
+                            "      <th>body_mass_g_sum</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Adelie</td>\n",
                             "      <td>Biscoe</td>\n",
                             "      <td>Female</td>\n",
                             "      <td>22</td>\n",
+                            "      <td>821.9</td>\n",
+                            "      <td>389.5</td>\n",
+                            "      <td>4118.0</td>\n",
+                            "      <td>74125.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Adelie</td>\n",
                             "      <td>Biscoe</td>\n",
                             "      <td>Male</td>\n",
                             "      <td>22</td>\n",
+                            "      <td>893.0</td>\n",
+                            "      <td>418.8</td>\n",
+                            "      <td>4189.0</td>\n",
+                            "      <td>89100.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>Adelie</td>\n",
                             "      <td>Dream</td>\n",
                             "      <td>Female</td>\n",
                             "      <td>27</td>\n",
+                            "      <td>996.6</td>\n",
+                            "      <td>475.7</td>\n",
+                            "      <td>5072.0</td>\n",
+                            "      <td>90300.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>Adelie</td>\n",
                             "      <td>Dream</td>\n",
                             "      <td>Male</td>\n",
                             "      <td>28</td>\n",
+                            "      <td>1122.0</td>\n",
+                            "      <td>527.5</td>\n",
+                            "      <td>5374.0</td>\n",
+                            "      <td>113275.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>Adelie</td>\n",
                             "      <td>Torgersen</td>\n",
                             "      <td>Female</td>\n",
                             "      <td>24</td>\n",
+                            "      <td>901.3</td>\n",
+                            "      <td>421.2</td>\n",
+                            "      <td>4519.0</td>\n",
+                            "      <td>81500.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>Adelie</td>\n",
                             "      <td>Torgersen</td>\n",
                             "      <td>Male</td>\n",
                             "      <td>23</td>\n",
+                            "      <td>933.5</td>\n",
+                            "      <td>446.0</td>\n",
+                            "      <td>4483.0</td>\n",
+                            "      <td>92800.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
                             "      <td>Chinstrap</td>\n",
                             "      <td>Dream</td>\n",
                             "      <td>Female</td>\n",
                             "      <td>34</td>\n",
+                            "      <td>1583.5</td>\n",
+                            "      <td>598.0</td>\n",
+                            "      <td>6519.0</td>\n",
+                            "      <td>119925.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
                             "      <td>Chinstrap</td>\n",
                             "      <td>Dream</td>\n",
                             "      <td>Male</td>\n",
                             "      <td>34</td>\n",
+                            "      <td>1737.2</td>\n",
+                            "      <td>654.6</td>\n",
+                            "      <td>6797.0</td>\n",
+                            "      <td>133925.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
                             "      <td>Gentoo</td>\n",
                             "      <td>Biscoe</td>\n",
                             "      <td>Female</td>\n",
                             "      <td>58</td>\n",
+                            "      <td>2642.7</td>\n",
+                            "      <td>825.8</td>\n",
+                            "      <td>12337.0</td>\n",
+                            "      <td>271425.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
                             "      <td>Gentoo</td>\n",
                             "      <td>Biscoe</td>\n",
                             "      <td>Male</td>\n",
                             "      <td>61</td>\n",
+                            "      <td>3017.9</td>\n",
+                            "      <td>958.8</td>\n",
+                            "      <td>13514.0</td>\n",
+                            "      <td>334575.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     species     island     sex   n\n",
-                            "0     Adelie     Biscoe  Female  22\n",
-                            "1     Adelie     Biscoe    Male  22\n",
-                            "2     Adelie      Dream  Female  27\n",
-                            "3     Adelie      Dream    Male  28\n",
-                            "4     Adelie  Torgersen  Female  24\n",
-                            "5     Adelie  Torgersen    Male  23\n",
-                            "6  Chinstrap      Dream  Female  34\n",
-                            "7  Chinstrap      Dream    Male  34\n",
-                            "8     Gentoo     Biscoe  Female  58\n",
-                            "9     Gentoo     Biscoe    Male  61"
+                            "     species     island     sex   n  bill_length_mm_sum  bill_depth_mm_sum  \\\n",
+                            "0     Adelie     Biscoe  Female  22               821.9              389.5   \n",
+                            "1     Adelie     Biscoe    Male  22               893.0              418.8   \n",
+                            "2     Adelie      Dream  Female  27               996.6              475.7   \n",
+                            "3     Adelie      Dream    Male  28              1122.0              527.5   \n",
+                            "4     Adelie  Torgersen  Female  24               901.3              421.2   \n",
+                            "5     Adelie  Torgersen    Male  23               933.5              446.0   \n",
+                            "6  Chinstrap      Dream  Female  34              1583.5              598.0   \n",
+                            "7  Chinstrap      Dream    Male  34              1737.2              654.6   \n",
+                            "8     Gentoo     Biscoe  Female  58              2642.7              825.8   \n",
+                            "9     Gentoo     Biscoe    Male  61              3017.9              958.8   \n",
+                            "\n",
+                            "   flipper_length_mm_sum  body_mass_g_sum  \n",
+                            "0                 4118.0          74125.0  \n",
+                            "1                 4189.0          89100.0  \n",
+                            "2                 5072.0          90300.0  \n",
+                            "3                 5374.0         113275.0  \n",
+                            "4                 4519.0          81500.0  \n",
+                            "5                 4483.0          92800.0  \n",
+                            "6                 6519.0         119925.0  \n",
+                            "7                 6797.0         133925.0  \n",
+                            "8                12337.0         271425.0  \n",
+                            "9                13514.0         334575.0  "
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "penguins.agg_df(type=['n'])"
+                "penguins.agg_df(type=['n','sum'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "id": "8686f087-2124-44e9-91dc-08350ea9a384",
             "metadata": {},
@@ -1105,19 +1161,26 @@
             "source": [
                 "penguins.long(col='features',\n",
                 "              value='value').wide(col='features',aggfunc='sum').long(col='features',value='value').value.sum()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "id": "9639866f-2f66-4f4e-aac7-e010649e4956",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "pivot_table is used with sum as agg because Index contains duplicate entries.\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -1474,27 +1537,27 @@
                             "22                NaN  \n",
                             "23                NaN  \n",
                             "24                NaN  \n",
                             "25                NaN  \n",
                             "26                NaN  "
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "penguins.long(col='features',\n",
                 "              value='value').wide(col='features')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 19,
             "id": "692ba49c-0d78-41d6-aad7-fa8045503ed7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1574,15 +1637,15 @@
                             "1  one   B    2   y\n",
                             "2  one   C    3   z\n",
                             "3  two   A    4   q\n",
                             "4  two   B    5   w\n",
                             "5  two   C    6   t"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = pd.DataFrame({'foo': ['one', 'one', 'one', 'two', 'two',\n",
                 "                           'two'],\n",
@@ -1590,15 +1653,15 @@
                 "                   'baz': [1, 2, 3, 4, 5, 6],\n",
                 "                   'zoo': ['x', 'y', 'z', 'q', 'w', 't']})\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 20,
             "id": "6502a2f3-0751-4d89-b400-74e99a635f18",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1685,27 +1748,106 @@
                             "1  one   y  NaN  2.0  NaN\n",
                             "2  one   z  NaN  NaN  3.0\n",
                             "3  two   q  4.0  NaN  NaN\n",
                             "4  two   t  NaN  NaN  6.0\n",
                             "5  two   w  NaN  5.0  NaN"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.wide(col='bar', value='baz')"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 21,
+            "id": "bc07e66a-a207-48aa-8d66-d23656fb4d21",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>type</th>\n",
+                            "      <th>mean_bill_length_cm</th>\n",
+                            "      <th>mean_body_mass_g</th>\n",
+                            "      <th>count</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>Gentoo</td>\n",
+                            "      <td>4.750488</td>\n",
+                            "      <td>5076.016260</td>\n",
+                            "      <td>124</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>Adelie</td>\n",
+                            "      <td>3.897500</td>\n",
+                            "      <td>3709.659091</td>\n",
+                            "      <td>44</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "     type  mean_bill_length_cm  mean_body_mass_g  count\n",
+                            "1  Gentoo             4.750488       5076.016260    124\n",
+                            "0  Adelie             3.897500       3709.659091     44"
+                        ]
+                    },
+                    "execution_count": 21,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "(penguins\n",
+                ".query(\"island == 'Biscoe'\")                                          #dplyr filter\n",
+                ".filter(items=['species', 'island', 'bill_length_mm', 'body_mass_g']) #dplyr select \n",
+                ".assign(bill_length_cm=lambda x: x.bill_length_mm / 10)               #dplyr mutate\n",
+                ".groupby(['species', 'island'])                                       #dplyr groupby\n",
+                ".agg(mean_bill_length_cm=('bill_length_cm', 'mean'),                  #dplyr summarize\n",
+                "     mean_body_mass_g=('body_mass_g', 'mean'),\n",
+                "     count=('species', 'size'))\n",
+                ".reset_index()                                                        #dplyr ungroup\n",
+                ".sort_values('mean_body_mass_g', ascending=False)                     #dplyr arrange\n",
+                ".drop(columns=['island'])                                             #dplyr select\n",
+                ".rename(columns={'species':'type'})                                   #dplyr rename\n",
+                ")\n"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": null,
-            "id": "a3c398fa-5ad4-48d6-8b9d-a3cbd173706d",
+            "id": "978a8e44-0b77-417e-bef3-988d1178d85f",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `pytae-2.1.5/src/.ipynb_checkpoints/recon-checkpoint.ipynb` & `pytae-2.2.0/src/recon.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'metadata'": "{'language_info': OrderedDict([('codemirror_mode', OrderedDict([('name', "*

 * *               "'ipython'), ('version', 3)])), ('file_extension', '.py'), ('mimetype', "*

 * *               "'text/x-python'), ('name', 'python'), ('nbconvert_exporter', 'python'), "*

 * *               "('pygments_lexer', 'ipython3'), ('version', '3.9.6')])}"}*

```diff
@@ -844,12 +844,24 @@
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "py_env",
             "language": "python",
             "name": "py_env"
+        },
+        "language_info": {
+            "codemirror_mode": {
+                "name": "ipython",
+                "version": 3
+            },
+            "file_extension": ".py",
+            "mimetype": "text/x-python",
+            "name": "python",
+            "nbconvert_exporter": "python",
+            "pygments_lexer": "ipython3",
+            "version": "3.9.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pytae-2.1.5/src/pytae/extend_pandas.py` & `pytae-2.2.0/src/pytae/extend_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,16 @@
     wide_df.columns.name = None
     
     return wide_df
 
 
 
 
+
+
 pd.DataFrame.clip = clip
 pd.DataFrame.agg_df = agg_df
 pd.DataFrame.long = long
 pd.DataFrame.wide = wide
 pd.DataFrame.handle_missing = handle_missing
 pd.DataFrame.return_join_table = return_join_table
 pd.DataFrame.cols = cols
```

### Comparing `pytae-2.1.5/src/pytae/general_utils.py` & `pytae-2.2.0/src/pytae/general_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -234,8 +234,46 @@
             file_list=u.return_file_list()
             if len(file_list)==1:
                 self.df = u.return_sample_df(file_list[0])        
             else:
                 print(str(file_list))
                 table = input('choose table without quote!\n')
                 self.df = u.return_sample_df(table)
-        return self.df
+        return self.df
+
+
+def getData(df, **kwargs):
+   
+    cols = list(kwargs.keys())
+    agg_cols=['value']
+    default_cols=[]
+
+    #manage agg cols
+    if 'value' in cols:
+        cols.remove('value')
+        agg_cols.remove('value')
+        if isinstance(kwargs['value'], list):  # Check if value is a list
+            agg_cols = kwargs['value']
+        else:
+            agg_cols = [kwargs['value']]  # If not a list, wrap it in a list
+
+    #manage default cols
+    if 'default_cols' in cols:
+        cols.remove('default_cols')
+        if isinstance(kwargs['default_cols'], list):  # Check if value is a list
+            default_cols=default_cols+  kwargs['default_cols']
+        else:
+            default_cols=default_cols+  [kwargs['default_cols']]  # If not a list, wrap it in a list
+
+    combined_cols=cols+default_cols
+   
+    #filter df
+    filtered_df = df[cols+default_cols+agg_cols].copy()
+    for c in cols:      
+        if isinstance(kwargs[c], list):
+            filtered_df = filtered_df[filtered_df[c].isin(kwargs[c])]
+        else:
+            filtered_df = filtered_df[filtered_df[c]==kwargs[c]]
+    #aggregate df
+    grouped_df = filtered_df.groupby(combined_cols,dropna=False)[agg_cols].agg('sum').reset_index()
+
+    return grouped_df
```

### Comparing `pytae-2.1.5/src/pytae/reconciller.py` & `pytae-2.2.0/src/pytae/reconciller.py`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/src/pytae/.ipynb_checkpoints/extend_pandas-checkpoint.py` & `pytae-2.2.0/src/pytae/.ipynb_checkpoints/extend_pandas-checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,16 @@
     wide_df.columns.name = None
     
     return wide_df
 
 
 
 
+
+
 pd.DataFrame.clip = clip
 pd.DataFrame.agg_df = agg_df
 pd.DataFrame.long = long
 pd.DataFrame.wide = wide
 pd.DataFrame.handle_missing = handle_missing
 pd.DataFrame.return_join_table = return_join_table
 pd.DataFrame.cols = cols
```

### Comparing `pytae-2.1.5/src/pytae/.ipynb_checkpoints/general_utils-checkpoint.py` & `pytae-2.2.0/src/pytae/.ipynb_checkpoints/general_utils-checkpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -234,8 +234,46 @@
             file_list=u.return_file_list()
             if len(file_list)==1:
                 self.df = u.return_sample_df(file_list[0])        
             else:
                 print(str(file_list))
                 table = input('choose table without quote!\n')
                 self.df = u.return_sample_df(table)
-        return self.df
+        return self.df
+
+
+def getData(df, **kwargs):
+   
+    cols = list(kwargs.keys())
+    agg_cols=['value']
+    default_cols=[]
+
+    #manage agg cols
+    if 'value' in cols:
+        cols.remove('value')
+        agg_cols.remove('value')
+        if isinstance(kwargs['value'], list):  # Check if value is a list
+            agg_cols = kwargs['value']
+        else:
+            agg_cols = [kwargs['value']]  # If not a list, wrap it in a list
+
+    #manage default cols
+    if 'default_cols' in cols:
+        cols.remove('default_cols')
+        if isinstance(kwargs['default_cols'], list):  # Check if value is a list
+            default_cols=default_cols+  kwargs['default_cols']
+        else:
+            default_cols=default_cols+  [kwargs['default_cols']]  # If not a list, wrap it in a list
+
+    combined_cols=cols+default_cols
+   
+    #filter df
+    filtered_df = df[cols+default_cols+agg_cols].copy()
+    for c in cols:      
+        if isinstance(kwargs[c], list):
+            filtered_df = filtered_df[filtered_df[c].isin(kwargs[c])]
+        else:
+            filtered_df = filtered_df[filtered_df[c]==kwargs[c]]
+    #aggregate df
+    grouped_df = filtered_df.groupby(combined_cols,dropna=False)[agg_cols].agg('sum').reset_index()
+
+    return grouped_df
```

### Comparing `pytae-2.1.5/src/pytae/.ipynb_checkpoints/reconciller-checkpoint.py` & `pytae-2.2.0/src/pytae/.ipynb_checkpoints/reconciller-checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/.gitignore` & `pytae-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/LICENSE` & `pytae-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytae-2.1.5/pyproject.toml` & `pytae-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytae"
-version = "2.1.5"
+version = "2.2.0"
 authors = [
   { name="Madhukar Kumar Jha", email="madhukar.k.jha@gmail.com" },
 ]
 description = "A package to enhance common day to day tasks in the life of a data scientist"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pytae-2.1.5/PKG-INFO` & `pytae-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytae
-Version: 2.1.5
+Version: 2.2.0
 Dynamic: Requires-Dist
 Summary: A package to enhance common day to day tasks in the life of a data scientist
 Project-URL: Homepage, https://github.com/maddytae/pytae
 Project-URL: Bug Tracker, https://github.com/maddytae/pytae/issues
 Author-email: Madhukar Kumar Jha <madhukar.k.jha@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

