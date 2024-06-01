# Comparing `tmp/mlable-0.2.2.tar.gz` & `tmp/mlable-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlable-0.2.2.tar", max compression
+gzip compressed data, was "mlable-0.3.1.tar", max compression
```

## Comparing `mlable-0.2.2.tar` & `mlable-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,22 @@
--rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.2.2/.github/README.md
--rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.2.2/mlable/__init__.py
--rw-r--r--   0        0        0     5219 2024-05-29 20:55:39.325361 mlable-0.2.2/mlable/blocks.py
--rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.2.2/mlable/data.py
--rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.2.2/mlable/initializers.py
--rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.2.2/mlable/io.py
--rw-r--r--   0        0        0    17525 2024-05-30 14:42:13.588855 mlable-0.2.2/mlable/layers.py
--rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.2.2/mlable/losses.py
--rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.2.2/mlable/optimizers.py
--rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.2.2/mlable/preprocessing/__init__.py
--rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.2.2/mlable/preprocessing/bpe.py
--rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.2.2/mlable/preprocessing/ngrams.py
--rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.2.2/mlable/sampling.py
--rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.2.2/mlable/summary.py
--rw-r--r--   0        0        0      433 2024-05-30 14:42:52.572822 mlable-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 mlable-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.3.1/.github/README.md
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.3.1/mlable/__init__.py
+-rw-r--r--   0        0        0    10479 2024-05-30 19:30:51.659026 mlable-0.3.1/mlable/__old__/layers.py
+-rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.3.1/mlable/data.py
+-rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.3.1/mlable/initializers.py
+-rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.3.1/mlable/io.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:09:00.732228 mlable-0.3.1/mlable/layers/__init__.py
+-rw-r--r--   0        0        0      952 2024-05-30 19:38:33.001975 mlable-0.3.1/mlable/layers/activation.py
+-rw-r--r--   0        0        0     3726 2024-05-31 19:27:13.842103 mlable-0.3.1/mlable/layers/embedding.py
+-rw-r--r--   0        0        0      983 2024-06-01 11:55:58.928431 mlable-0.3.1/mlable/layers/linear.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:27:52.982216 mlable-0.3.1/mlable/layers/regularization.py
+-rw-r--r--   0        0        0     4410 2024-05-30 18:16:44.775596 mlable-0.3.1/mlable/layers/reshaping.py
+-rw-r--r--   0        0        0     5930 2024-06-01 12:42:33.264514 mlable-0.3.1/mlable/layers/transformer.py
+-rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.3.1/mlable/losses.py
+-rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.3.1/mlable/optimizers.py
+-rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.3.1/mlable/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.3.1/mlable/preprocessing/bpe.py
+-rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.3.1/mlable/preprocessing/ngrams.py
+-rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.3.1/mlable/sampling.py
+-rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.3.1/mlable/summary.py
+-rw-r--r--   0        0        0      433 2024-06-01 11:11:33.111311 mlable-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 mlable-0.3.1/PKG-INFO
```

### Comparing `mlable-0.2.2/mlable/blocks.py` & `mlable-0.3.1/mlable/layers/transformer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,135 @@
 import tensorflow as tf
 
 # FEED FORWARD BLOCK ##########################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class ResidualFeedForwardBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         hidden_dim: int,
         normalization_epsilon: float=0.001,
         **kwargs
-    ):
+    ) -> None:
+        # init
         super(ResidualFeedForwardBlock, self).__init__(**kwargs)
-        self._normalization = tf.keras.layers.LayerNormalization(axis=-1, epsilon=normalization_epsilon, center=True, scale=True, beta_initializer='zeros', gamma_initializer='glorot_uniform', beta_regularizer=None, gamma_regularizer=None, beta_constraint=None, gamma_constraint=None,  **kwargs)
-        self._hidden_dim = hidden_dim
-        self._hidden = tf.keras.layers.Dense(units=self._hidden_dim, activation='relu', use_bias=True, kernel_initializer='glorot_uniform', bias_initializer='zeros', kernel_regularizer=None, bias_regularizer=None, activity_regularizer=None, kernel_constraint=None, bias_constraint=None, **kwargs)
+        # config
+        self._config = {
+            'hidden_dim': hidden_dim,
+            'normalization_epsilon': normalization_epsilon}
+        # layers
+        self._normalization = tf.keras.layers.LayerNormalization(axis=-1, epsilon=normalization_epsilon, center=True, scale=True, beta_initializer='zeros', gamma_initializer='glorot_normal')
+        self._hidden = tf.keras.layers.Dense(units=hidden_dim, activation='relu', use_bias=True, kernel_initializer='glorot_normal', bias_initializer='zeros')
         self._projection = None
 
     def build(self, input_shape: tuple, **kwargs) -> None:
         # create the projection layer to match the input shape
-        self._projection = tf.keras.layers.Dense(units=input_shape[-1], activation=None, use_bias=True, kernel_initializer='glorot_uniform', bias_initializer='zeros', kernel_regularizer=None, bias_regularizer=None, activity_regularizer=None, kernel_constraint=None, bias_constraint=None, **kwargs)
+        self._projection = tf.keras.layers.Dense(units=input_shape[-1], activation='linear', use_bias=True, kernel_initializer='glorot_normal', bias_initializer='zeros')
         # no need to build the activation layer
         self._normalization.build(input_shape) # no weights
         self._hidden.build(input_shape) # (C, H)
         self._projection.build(list(input_shape)[:-1] + [self._hidden_dim]) # (H, C), called on (x * W_h) => shape (B, T, H)
         # notify the model
         self.built = True
 
-    def call(self, inputs: tf.Tensor):
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
         __dx = inputs # (B, T, C)
         # normalize the features
         __dx = self._normalization(__dx) # (B, T, C)
         # expand inside the hidden layer
         __dx = self._hidden(__dx) # (B, T, C) * (C, H) = (B, T, H)
         # projection: match the input shape
         __dx = self._projection(__dx) # (B, T, H) * (H, C) = (B, T, C)
         # residual
         return inputs + __dx # (B, T, C)
 
+    def get_config(self) -> dict:
+        __parent_config = super(ResidualFeedForwardBlock, self).get_config()
+        return {**__parent_config, **self._config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # ATTENTION BLOCK #############################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class ResidualSelfAttentionBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         attention_head_dim: int,
         attention_head_count: int=1,
         normalization_epsilon: float=0.001,
         dropout: float=0.0,
         **kwargs
-    ):
+    ) -> None:
+        # init
         super(ResidualSelfAttentionBlock, self).__init__(**kwargs)
-        self._normalization = tf.keras.layers.LayerNormalization(axis=-1, epsilon=normalization_epsilon, center=True, scale=True, beta_initializer='zeros', gamma_initializer='glorot_uniform', beta_regularizer=None, gamma_regularizer=None, beta_constraint=None, gamma_constraint=None,  **kwargs)
-        self._attention = tf.keras.layers.MultiHeadAttention(num_heads=attention_head_count, key_dim=attention_head_dim, value_dim=attention_head_dim, dropout=dropout, use_bias=True, output_shape=None, attention_axes=None, kernel_initializer='glorot_uniform', bias_initializer='zeros', kernel_regularizer=None, bias_regularizer=None, activity_regularizer=None, kernel_constraint=None, bias_constraint=None, **kwargs)
-
-    def build(self, input_shape: tuple, **kwargs) -> None:
-        # build
-        self._normalization.build(input_shape)
-        self._attention.build(input_shape, input_shape)
-        # notify the model
-        self.built = True
+        # config
+        self._config = {
+            'attention_head_dim': attention_head_dim,
+            'attention_head_count': attention_head_count,
+            'normalization_epsilon': normalization_epsilon,
+            'dropout': dropout}
+        # layers
+        self._normalization = tf.keras.layers.LayerNormalization(axis=-1, epsilon=normalization_epsilon, center=True, scale=True, beta_initializer='zeros', gamma_initializer='glorot_normal')
+        self._attention = tf.keras.layers.MultiHeadAttention(num_heads=attention_head_count, key_dim=attention_head_dim, value_dim=attention_head_dim, dropout=dropout, use_bias=True, kernel_initializer='glorot_normal', bias_initializer='zeros')
 
-    def call(self, inputs: tf.Tensor):
+    def call(self, inputs: tf.Tensor)  -> tf.Tensor:
         __dx = inputs # (B, T, C)
         # normalize the features
         __dx = self._normalization(__dx) # (B, T, C)
         # self-attention
         __dx = self._attention(key=__dx, query=__dx, value=__dx, return_attention_scores=False, use_causal_mask=True) # (B, T, H_d * H_c) = (B, T, C) use_causal_mask=True
         # residual
         return inputs + __dx # (B, T, C)
 
+    def get_config(self) -> dict:
+        __parent_config = super(ResidualSelfAttentionBlock, self).get_config()
+        return {**__parent_config, **self._config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # META BLOCK ##################################################################
 
+@keras.saving.register_keras_serializable(package='layers')
 class ResidualSelfAttentionDecoderBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         hidden_dim: int,
         attention_head_dim: int,
         attention_head_count: int=1,
         normalization_epsilon: float=0.001,
         dropout: float=0.0,
         **kwargs
-    ):
+    ) -> None:
+        # init
         super(ResidualSelfAttentionDecoderBlock, self).__init__(**kwargs)
+        # config
+        self._config = {
+            'hidden_dim': hidden_dim,
+            'attention_head_dim': attention_head_dim,
+            'attention_head_count': attention_head_count,
+            'normalization_epsilon': normalization_epsilon,
+            'dropout': dropout}
+        # layers
         self._feedforward = ResidualFeedForwardBlock(hidden_dim=hidden_dim, normalization_epsilon=normalization_epsilon)
         self._attention = ResidualSelfAttentionBlock(attention_head_dim=attention_head_dim, attention_head_count=attention_head_count, normalization_epsilon=normalization_epsilon, dropout=dropout)
 
-    def build(self, input_shape: tuple, **kwargs) -> None:
-        self._feedforward.build(input_shape)
-        self._attention.build(input_shape)
-        # notify the model
-        self.built = True
-
-    def call(self, inputs: tf.Tensor):
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
         __dx = inputs # (B, T, C)
         # residual self-attention
         __dx = self._attention(__dx) # (B, T, C)
         # residual FF
         __dx = self._feedforward(__dx) # (B, T, C)
         # residual
         return __dx # (B, T, C)
+
+    def get_config(self) -> dict:
+        __parent_config = super(ResidualSelfAttentionDecoderBlock, self).get_config()
+        return {**__parent_config, **self._config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
```

### Comparing `mlable-0.2.2/mlable/initializers.py` & `mlable-0.3.1/mlable/initializers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/mlable/io.py` & `mlable-0.3.1/mlable/io.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/mlable/layers.py` & `mlable-0.3.1/mlable/__old__/layers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,58 @@
 import keras
 import numpy as np
 import tensorflow as tf
 
+# ACTIVATIONS #################################################################
+
+@keras.saving.register_keras_serializable(package='layers')
+class Softmax(tf.keras.layers.Layer):
+    def __init__(
+        self,
+        axis: int=-1,
+        **kwargs
+    ):
+        super(Softmax, self).__init__(**kwargs)
+        self._config = {'axis': axis}
+
+    def call(self, inputs: tf.Tensor, **kwargs):
+        return tf.nn.softmax(inputs, axis=self._config['axis'])
+
+    def get_config(self) -> dict:
+        __parent_config = super(Softmax, self).get_config()
+        return {**__parent_config, **self._config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
+
 # NORMALIZATION ###############################################################
 
 @keras.saving.register_keras_serializable(package='layers')
 class BatchNormalization(tf.keras.layers.Layer):
     def __init__(
         self,
         axis: int=0,
         momentum: float=0.99,
         epsilon: float=0.001,
         **kwargs
     ):
         super(BatchNormalization, self).__init__(**kwargs)
-        self._axis = axis
-        self._momentum = momentum
-        self._epsilon = epsilon
+        self._config = {
+            'axis': axis,
+            'momentum': momentum,
+            'epsilon': epsilon,}
         self._mean = None
         self._stddev = None
         self._gain = None
         self._bias = None
 
     def build(self, input_shape: tuple):
         # shape
-        __axis = self._axis % len(input_shape) # positive index even when the axis is specified negatively, like -2
+        __axis = self._config['axis'] % len(input_shape) # positive index even when the axis is specified negatively, like -2
         __shape = [1 if __i == __axis else __d for __i, __d in enumerate(input_shape)]
         # values
         __mean_init = tf.keras.initializers.GlorotNormal()
         __stddev_init = tf.keras.initializers.GlorotNormal()
         __gain_init = tf.keras.initializers.GlorotNormal()
         __bias_init = tf.keras.initializers.Zeros()
         # tensors
@@ -38,47 +62,44 @@
         self._bias = self.add_weight("bias", shape=__shape, initializer=__bias_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor, training: bool=True, **kwargs):
         if training:
             # current values
-            __batch_mean = tf.math.reduce_mean(inputs, axis=self._axis, keepdims=True)
-            __batch_stddev = tf.math.reduce_std(inputs, axis=self._axis, keepdims=True)
+            __batch_mean = tf.math.reduce_mean(inputs, axis=self._config['axis'], keepdims=True)
+            __batch_stddev = tf.math.reduce_std(inputs, axis=self._config['axis'], keepdims=True)
             # update parameters
-            self._mean = tf.stop_gradient(self._momentum * self._mean + (1. - self._momentum) * __batch_mean)
-            self._stddev = tf.stop_gradient(self._momentum * self._stddev + (1. - self._momentum) * __batch_stddev)
+            self._mean = tf.stop_gradient(self._config['momentum'] * self._mean + (1. - self._config['momentum']) * __batch_mean)
+            self._stddev = tf.stop_gradient(self._config['momentum'] * self._stddev + (1. - self._config['momentum']) * __batch_stddev)
         # normalize
-        __normalized = tf.math.divide(inputs - self._mean, self._stddev + self._epsilon)
+        __normalized = tf.math.divide(inputs - self._mean, self._stddev + self._config['epsilon'])
         # scale
         return tf.math.multiply(self._gain, __normalized) + self._bias
 
     def get_config(self) -> dict:
         __parent_config = super(BatchNormalization, self).get_config()
-        __child_config = {
-            'axis': self._axis,
-            'momentum': self._momentum,
-            'epsilon': self._epsilon}
-        return {**__parent_config, **__child_config}
+        return {**__parent_config, **self._config}
 
     @classmethod
     def from_config(cls, config) -> tf.keras.layers.Layer:
         return cls(**config)
 
 @keras.saving.register_keras_serializable(package='layers')
 class LayerNormalization(tf.keras.layers.Layer):
     def __init__(
         self,
         axis: int=-1,
         epsilon: float=0.001,
         **kwargs
     ):
         super(LayerNormalization, self).__init__(**kwargs)
-        self._axis = axis
-        self._epsilon = epsilon
+        self._config= {
+            'axis': axis,
+            'epsilon': epsilon,}
         self._gain = None
         self._bias = None
 
     def build(self, input_shape: tuple):
         # shape
         __shape = [1] + input_shape[1:]
         # values
@@ -88,77 +109,103 @@
         self._gain = self.add_weight("gain", shape=__shape, initializer=__gain_init)
         self._bias = self.add_weight("bias", shape=__shape, initializer=__bias_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor, training: bool=True, **kwargs):
         # current values
-        __layer_mean = tf.math.reduce_mean(inputs, axis=self._axis, keepdims=True)
-        __layer_stddev = tf.math.reduce_std(inputs, axis=self._axis, keepdims=True)
+        __layer_mean = tf.math.reduce_mean(inputs, axis=self._config['axis'], keepdims=True)
+        __layer_stddev = tf.math.reduce_std(inputs, axis=self._config['axis'], keepdims=True)
         # normalize
-        __normalized = tf.math.divide(inputs - __layer_mean, __layer_stddev + self._epsilon)
+        __normalized = tf.math.divide(inputs - __layer_mean, __layer_stddev + self._config['epsilon'])
         # scale
         return tf.math.add(tf.math.multiply(self._gain, __normalized), self._bias)
 
     def get_config(self) -> dict:
         __parent_config = super(LayerNormalization, self).get_config()
-        __child_config = {
-            'axis': self._axis,
-            'epsilon': self._epsilon}
-        return {**__parent_config, **__child_config}
+        return {**__parent_config, **self._config}
 
     @classmethod
     def from_config(cls, config) -> tf.keras.layers.Layer:
         return cls(**config)
 
-# REGULARIZATION ##############################################################
-
-# dropout
-
 # LINEAR ######################################################################
 
 @keras.saving.register_keras_serializable(package='layers')
 class Dense(tf.keras.layers.Layer):
     def __init__(
         self,
         units: int,
         use_bias: bool=True,
         **kwargs
     ):
         super(Dense, self).__init__(**kwargs)
-        self._units = units
-        self._biased = use_bias
+        self._config = {
+            'units': units,
+            'use_bias': use_bias,}
         self._kernel = None
         self._bias = None
 
     def build(self, input_shape: tuple):
         # kernel
         __kernel_init = tf.keras.initializers.GlorotNormal()
-        self._kernel = self.add_weight("kernel", shape=[int(input_shape[-1]), self._units], initializer=__kernel_init)
+        self._kernel = self.add_weight("kernel", shape=[int(input_shape[-1]), self._config['units']], initializer=__kernel_init)
         # bias
-        if self._biased:
+        if self._config['use_bias']:
             __bias_init = tf.keras.initializers.Zeros()
-            self._bias = self.add_weight("bias", shape=[self._units], initializer=__bias_init)
+            self._bias = self.add_weight("bias", shape=[self._config['units']], initializer=__bias_init)
         # notify the model
         self.built = True
 
     def call(self, inputs: tf.Tensor, **kwargs):
-        return tf.matmul(inputs, self._kernel) + self._bias if (self._biased and self._bias is not None) else tf.matmul(inputs, self._kernel)
+        return tf.matmul(inputs, self._kernel) + self._bias if (self._config['use_bias'] and self._bias is not None) else tf.matmul(inputs, self._kernel)
 
     def get_config(self) -> dict:
         __parent_config = super(Dense, self).get_config()
-        __child_config = {
-            'units': self._units,
-            'use_bias': self._biased}
-        return {**__parent_config, **__child_config}
+        return {**__parent_config, **self._config}
 
     @classmethod
     def from_config(cls, config) -> tf.keras.layers.Layer:
         return cls(**config)
 
+# EMBEDDING ###################################################################
+
+@keras.saving.register_keras_serializable(package='layers')
+class Embedding(tf.keras.layers.Layer):
+    def __init__(
+        self,
+        input_dim: int,
+        output_dim: int,
+        **kwargs
+    ):
+        super(Embedding, self).__init__(**kwargs)
+        self._config = {
+            'input_dim': input_dim,
+            'output_dim': output_dim,}
+        self._kernel = None
+
+    def build(self, input_shape: tuple):
+        __kernel_init = tf.keras.initializers.GlorotNormal()
+        # register the weights
+        self._kernel = self.add_weight(name="kernel", shape=[self._config['input_dim'], self._config['output_dim']], initializer=__kernel_init)
+        # notify the model
+        self.built = True
+
+    def call(self, inputs: tf.Tensor, **kwargs):
+        # content embedding
+        __x = tf.one_hot(indices=inputs, depth=self._config['input_dim'], dtype=tf.dtypes.float32)
+        return tf.matmul(__x, self._kernel)
+
+    def get_config(self) -> dict:
+        __parent_config = super(Embedding, self).get_config()
+        return {**__parent_config, **self._config}
+
+    @classmethod
+    def from_config(cls, config) -> tf.keras.layers.Layer:
+        return cls(**config)
 # QUADRATIC ###################################################################
 
 @keras.saving.register_keras_serializable(package='layers')
 class Attention(tf.keras.layers.Layer):
     def __init__(
         self,
         head_dim: int,
@@ -212,256 +259,7 @@
             'head_dim': self._head_dim,
             'head_count': self._head_count}
         return {**__parent_config, **__child_config}
 
     @classmethod
     def from_config(cls, config) -> tf.keras.layers.Layer:
         return cls(**config)
-
-# EMBEDDING ###################################################################
-
-@keras.saving.register_keras_serializable(package='layers')
-class Embedding(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        input_dim: int,
-        output_dim: int,
-        **kwargs
-    ):
-        super(Embedding, self).__init__(**kwargs)
-        self._input_dim = input_dim
-        self._output_dim = output_dim
-        self._kernel = None
-
-    def build(self, input_shape: tuple):
-        __kernel_init = tf.keras.initializers.GlorotNormal()
-        # register the weights
-        self._kernel = self.add_weight(name="kernel", shape=[self._input_dim, self._output_dim], initializer=__kernel_init)
-        # notify the model
-        self.built = True
-
-    def call(self, inputs: tf.Tensor, **kwargs):
-        # content embedding
-        __x = tf.one_hot(indices=inputs, depth=self._input_dim, dtype=tf.dtypes.float32)
-        return tf.matmul(__x, self._kernel)
-
-    def get_config(self) -> dict:
-        __parent_config = super(Embedding, self).get_config()
-        __child_config = {
-            'input_dim': self._input_dim,
-            'output_dim': self._output_dim}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        return cls(**config)
-
-@keras.saving.register_keras_serializable(package='layers')
-class PositionalEmbedding(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        input_axis: int=1, # axis of the sequence
-        output_axis: int=-1, # axis of the embedding
-        **kwargs
-    ):
-        super(PositionalEmbedding, self).__init__(**kwargs)
-        self._input_axis = input_axis
-        self._output_axis = output_axis
-        self._kernel = None
-
-    def build(self, input_shape: tuple) -> None:
-        # shape
-        __axes = [self._input_axis % len(input_shape), self._output_axis % len(input_shape)]
-        __shape = [(__d if __i in __axes else 1) for __i, __d in enumerate(list(input_shape))]
-        # init values
-        __kernel_init = tf.keras.initializers.GlorotNormal()
-        # register the weights
-        self._kernel = self.add_weight(name="kernel", shape=__shape, initializer=__kernel_init)
-        # notify the model
-        self.built = True
-
-    def call(self, inputs: tf.Tensor) -> tf.Tensor:
-        return inputs + self._kernel # each index in the sequence axis has a dedicated bias (different from dense bias)
-
-    def get_config(self) -> dict:
-        __parent_config = super(PositionalEmbedding, self).get_config()
-        __child_config = {
-            'input_axis': self._input_axis,
-            'output_axis': self._output_axis}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        return cls(**config)
-
-# RESIDUALS ###################################################################
-
-# ACTIVATION ##################################################################
-
-@keras.saving.register_keras_serializable(package='layers')
-class Activation(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        function: callable,
-        **kwargs
-    ):
-        super(Activation, self).__init__(**kwargs)
-        self._function = function
-
-    def call(self, inputs: tf.Tensor, **kwargs):
-        return self._function(inputs)
-
-    def get_config(self) -> dict:
-        __parent_config = super(Activation, self).get_config()
-        __child_config = {'function': keras.saving.serialize_keras_object(self._function),}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        __fn_config = config.pop('function')
-        __fn = keras.saving.deserialize_keras_object(__fn_config)
-        return cls(function=__fn, **config)
-
-@keras.saving.register_keras_serializable(package='layers')
-class Softmax(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        axis: int=-1,
-        **kwargs
-    ):
-        super(Softmax, self).__init__(**kwargs)
-        self._axis = axis
-
-    def call(self, inputs: tf.Tensor, **kwargs):
-        return tf.nn.softmax(inputs, axis=self._axis)
-
-    def get_config(self) -> dict:
-        __parent_config = super(Softmax, self).get_config()
-        __child_config = {'axis': self._axis,}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        return cls(**config)
-
-# RESHAPING ###################################################################
-
-def _normalize_shape(shape: list) -> list:
-    return [-1 if __d is None else __d for __d in shape]
-
-def _normalize_dim(dim: int) -> int:
-    return -1 if (dim is None or dim < 0) else dim
-
-def _multiply_dim(dim_l: int, dim_r: int) -> int:
-    return -1 if (dim_l == -1 or dim_r == -1) else dim_l * dim_r
-
-def _divide_dim(dim_l: int, dim_r: int) -> int:
-    return -1 if (dim_l == -1 or dim_r == -1) else dim_l // dim_r
-
-@keras.saving.register_keras_serializable(package='layers')
-class Divide(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        input_axis: int, # relative to the NEW shape / rank
-        output_axis: int, # same
-        factor: int,
-        insert: bool=False,
-        **kwargs
-    ) -> None:
-        super(Divide, self).__init__(**kwargs)
-        self._input_axis = input_axis
-        self._output_axis = output_axis
-        self._factor = factor
-        self._insert = insert
-
-    def call(self, inputs: tf.Tensor) -> tf.Tensor:
-        # infer the dimension of the symbolic axis
-        __shape = _normalize_shape(list(inputs.shape))
-        # rank, according to the new shape
-        __rank = len(__shape) + int(self._insert)
-        # axes, taken from the new shape
-        __axis0 = self._input_axis % __rank
-        __axis1 = self._output_axis % __rank
-        # option to group data on a new axis
-        if self._insert: __shape.insert(__axis1, 1)
-        # move data from axis 0 to axis 1
-        __shape[__axis0] = _divide_dim(__shape[__axis0], self._factor)
-        __shape[__axis1] = _multiply_dim(__shape[__axis1], self._factor)
-        return tf.reshape(tensor=inputs, shape=__shape)
-
-    def get_config(self) -> dict:
-        __parent_config = super(Divide, self).get_config()
-        __child_config = {
-            'input_axis': self._input_axis,
-            'output_axis': self._output_axis,
-            'factor': self._factor,
-            'insert': self._insert}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        return cls(**config)
-
-@keras.saving.register_keras_serializable(package='layers')
-class Merge(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        left_axis: int=-2,
-        right_axis: int=-1,
-        left: bool=True,
-        **kwargs
-    ) -> None:
-        super(Merge, self).__init__(**kwargs)
-        self._left_axis = left_axis
-        self._right_axis = right_axis
-        self._left = left
-
-    def call(self, inputs: tf.Tensor) -> tf.Tensor:
-        # infer the dimension of the symbolic axis
-        __shape = _normalize_shape(list(inputs.shape))
-        __rank = len(__shape)
-        # target axes
-        __axis_l = self._left_axis % __rank
-        __axis_r = self._right_axis % __rank
-        # new axis
-        __dim = _multiply_dim(__shape[__axis_l], __shape[__axis_r])
-        __axis_k = __axis_l if self._left else __axis_r # kept axis
-        __axis_d = __axis_r if self._left else __axis_l # deleted axis
-        # new shape
-        __shape[__axis_k] = __dim
-        __shape.pop(__axis_d)
-        # actually merge the two axes
-        return tf.reshape(tensor=inputs, shape=__shape)
-
-    def get_config(self) -> dict:
-        __parent_config = super(Merge, self).get_config()
-        __child_config = {
-            'left_axis': self._left_axis,
-            'right_axis': self._right_axis,
-            'left': self._left}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        return cls(**config)
-
-@keras.saving.register_keras_serializable(package='layers')
-class Reshape(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        target_shape: tuple,
-        **kwargs
-    ) -> None:
-        super(Reshape, self).__init__(**kwargs)
-        self._shape = target_shape
-
-    def call(self, inputs: tf.Tensor, **kwargs) -> tf.Tensor:
-        return tf.reshape(inputs, self._shape)
-
-    def get_config(self) -> dict:
-        __parent_config = super(Reshape, self).get_config()
-        __child_config = {'target_shape': self._shape,}
-        return {**__parent_config, **__child_config}
-
-    @classmethod
-    def from_config(cls, config) -> tf.keras.layers.Layer:
-        return cls(**config)
```

### Comparing `mlable-0.2.2/mlable/optimizers.py` & `mlable-0.3.1/mlable/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/mlable/preprocessing/bpe.py` & `mlable-0.3.1/mlable/preprocessing/bpe.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/mlable/preprocessing/ngrams.py` & `mlable-0.3.1/mlable/preprocessing/ngrams.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/mlable/sampling.py` & `mlable-0.3.1/mlable/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/mlable/summary.py` & `mlable-0.3.1/mlable/summary.py`

 * *Files identical despite different names*

### Comparing `mlable-0.2.2/PKG-INFO` & `mlable-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlable
-Version: 0.2.2
+Version: 0.3.1
 Summary: Tensorflow libs: layers, blocks, optimizers, etc.
 Author: apehex
 Author-email: apehex@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

