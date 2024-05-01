# Comparing `tmp/connectome_interpreter-1.6.5.tar.gz` & `tmp/connectome_interpreter-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.6.5.tar", last modified: Mon Apr 29 23:41:39 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.7.0.tar", last modified: Wed May  1 16:04:01 2024, max compression
```

## Comparing `connectome_interpreter-1.6.5.tar` & `connectome_interpreter-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 23:41:39.534208 connectome_interpreter-1.6.5/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.5/LICENSE
--rw-rw-rw-   0        0        0     1066 2024-04-29 23:41:39.532213 connectome_interpreter-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 23:41:39.482272 connectome_interpreter-1.6.5/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.5/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    34367 2024-04-29 23:38:47.000000 connectome_interpreter-1.6.5/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.5/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.6.5/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.5/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 23:41:39.523908 connectome_interpreter-1.6.5/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1066 2024-04-29 23:41:39.000000 connectome_interpreter-1.6.5/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-29 23:41:39.000000 connectome_interpreter-1.6.5/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 23:41:39.000000 connectome_interpreter-1.6.5/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-04-29 23:41:39.000000 connectome_interpreter-1.6.5/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-29 23:41:39.000000 connectome_interpreter-1.6.5/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 23:41:39.534208 connectome_interpreter-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     2068 2024-04-29 23:36:32.000000 connectome_interpreter-1.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 23:41:39.529886 connectome_interpreter-1.6.5/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.5/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.5/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.5/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.642562 connectome_interpreter-1.7.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     1066 2024-05-01 16:04:01.641560 connectome_interpreter-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.595155 connectome_interpreter-1.7.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.7.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    35488 2024-05-01 12:12:06.000000 connectome_interpreter-1.7.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    22184 2024-05-01 14:15:27.000000 connectome_interpreter-1.7.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.7.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    32941 2024-05-01 15:50:45.000000 connectome_interpreter-1.7.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.623706 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1066 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:04:01.642562 connectome_interpreter-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-05-01 15:57:55.000000 connectome_interpreter-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.639411 connectome_interpreter-1.7.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.7.0/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.7.0/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.6.5/LICENSE` & `connectome_interpreter-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.5/PKG-INFO` & `connectome_interpreter-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.6.5
+Version: 1.7.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.6.5/README.md` & `connectome_interpreter-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.5/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.7.0/connectome_interpreter/activation_maximisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,16 @@
 
         # stack the numpy activations together
         self.activations = torch.stack(self.activations, dim=1)
         return self.activations
 
 
 def activation_maximisation(
-        model, selected_neurons_per_layer: Dict[int, List[int]],
+        model, neurons_to_activate: Dict[int, List[int]],
+        neurons_to_deactivate=None,
         input_tensor=None,
         num_iterations=100, learning_rate=0.4,
         in_regularisation_lambda=0.1, custom_in_regularisation: Callable[[torch.Tensor], torch.Tensor] = None,
         out_regularisation_lambda=0.1,
         early_stopping=True, stopping_threshold=1e-6, n_runs=10,
         use_tqdm=True, print_output=True, report_memory_usage=False,
         device=None, wandb=True) -> Tuple[np.ndarray, np.ndarray, list, list]:
@@ -131,16 +132,18 @@
 
     This method adjusts `input_tensor` over `num_iterations` to maximize the activation of specified neurons in `model`,
     while also applying custom regularization to the input and output. The function supports early stopping based on a threshold
     to prevent unnecessary computations if the activation change becomes negligible.
 
     Args:
         model: A PyTorch model with `activations`, `sensory_indices`, and `threshold` attributes.
-        selected_neurons_per_layer (Dict[int, List[int]]): A dictionary mapping from layer indices to lists of neuron indices
+        neurons_to_activate (Dict[int, List[int]]): A dictionary mapping from layer indices to lists of neuron indices
             whose activations are to be maximized.
+        neurons_to_deactivate (Dict[int, List[int]]): A dictionary mapping from layer indices to lists of neuron indices
+            whose activations are to be minimized. Defaults to None.
         input_tensor (torch.Tensor, optional): The initial tensor to optimize. If None, a random tensor is created.
             Defaults to None.
         num_iterations (int, optional): The number of iterations to run the optimization for. Defaults to 100.
         learning_rate (float, optional): The learning rate for the optimizer. Defaults to 0.01.
         in_regularisation_lambda (float, optional): The regularization coefficient for punishing input neuron activation. Defaults to 0.4.
         custom_in_regularisation (Callable[[torch.Tensor], torch.Tensor], optional): A function that applies custom
             regularization to the `input_tensor`. Defaults to L1+L2 norm if None.
@@ -224,42 +227,55 @@
                                 snapshot, 0)  # Thresholded ReLU
             # Limit the range between 0 and 1
             snapshot = np.tanh(snapshot)
             input_snapshots.append(snapshot)
 
         # Calculate activation loss
         activation_loss = torch.tensor(0.0, device=input_tensor.device)
-
-        for layer_index, neuron_indices in selected_neurons_per_layer.items():
+        for layer_index, neuron_indices in neurons_to_activate.items():
             # Ensure layer index is valid
             if layer_index < model.activations.shape[1]:
                 # Get activations for this layer
                 layer_activations = model.activations[:, layer_index]
                 # Negative sign because we want to maximize activation
                 # Only select activations from specified neurons
-                # layer_activations is now a numpy array
                 activation_loss -= torch.mean(
                     layer_activations[neuron_indices])
+            else:
+                print(f"Layer index {layer_index} is invalid. Skipping.")
         # in the end, activation loss is the sum of mean activation across layers.
 
+        silence_loss = torch.tensor(0.0, device=input_tensor.device)
+        if neurons_to_deactivate is not None:
+            for layer_index, neuron_indices in neurons_to_deactivate.items():
+                # Ensure layer index is valid
+                if layer_index < model.activations.shape[1]:
+                    # Get activations for this layer
+                    layer_activations = model.activations[:, layer_index]
+                    # Only select activations from specified neurons
+                    silence_loss += torch.mean(
+                        layer_activations[neuron_indices])
+
         out_regularisation_loss = out_regularisation_lambda * torch.mean(
             model.activations)
         # Apply custom regularisation
         in_regularisation_loss = in_regularisation_lambda * custom_in_regularisation(
             input_tensor)
-        loss = activation_loss + in_regularisation_loss + out_regularisation_loss
+        loss = activation_loss + silence_loss + \
+            in_regularisation_loss + out_regularisation_loss
         losses.append(loss.item())
 
         if early_stopping and (iteration > n_runs):
             # when the difference between the max and the min < stopping_threshold
             if np.max(losses[-n_runs:]) - np.min(losses[-n_runs:]) < stopping_threshold:
                 break
 
         if wandb:
             dct = {"activation_loss": activation_loss.item(),
+                   "silence_loss": silence_loss.item(),
                    "in_regularisation_loss": in_regularisation_loss.item(),
                    'out_regularisation_loss': out_regularisation_loss.item(),
                    "loss": loss.item()}
             wandb.log(dct)
 
         act_loss.append(activation_loss.item())
         out_reg_loss.append(out_regularisation_loss.item())
@@ -268,15 +284,15 @@
         # Backward pass and optimization
         loss.backward()
         optimizer.step()
 
         # Optional: Print information about the optimization process
         if print_output and iteration % 10 == 0:  # Print every 10 iterations
             print(
-                f"Iteration {iteration}: Activation Loss = {activation_loss.item()}, Input regularization Loss = {in_regularisation_loss.item()}, Output regularization Loss = {out_regularisation_loss.item()}")
+                f"Iteration {iteration}: Activation Loss = {activation_loss.item()}, De-activation loss = {silence_loss.item()}, Input regularization Loss = {in_regularisation_loss.item()}, Output regularization Loss = {out_regularisation_loss.item()}")
 
         if report_memory_usage and iteration % 10 == 0:
             print(f'GPU memory at iteration {iteration}:', torch.cuda.memory_allocated(
                 device) / 1e9, 'GB')
 
         torch.cuda.empty_cache()
 
@@ -409,15 +425,15 @@
 #             self.activations.append(x)
 
 #         self.activations = torch.stack(self.activations, dim=1)
 #         return self.activations
 
 
 # def activation_maximisation(
-#         model, selected_neurons_per_layer: Dict[int, List[int]],
+#         model, neurons_to_activate: Dict[int, List[int]],
 #         input_tensor=None,
 #         num_iterations=300, learning_rate=0.4,
 #         in_regularisation_lambda=0.1, custom_in_regularisation: Callable[[torch.Tensor], torch.Tensor] = None,
 #         out_regularisation_lambda=0.1,
 #         early_stopping=True, stopping_threshold=1e-6, n_runs=10,
 #         use_tqdm=True, print_output=True,
 #         device=None, wandb=True) -> Tuple[np.ndarray, np.ndarray, list, list]:
@@ -426,15 +442,15 @@
 
 #     This method adjusts `input_tensor` over `num_iterations` to maximize the activation of specified neurons in `model`,
 #     while also applying custom regularization to the input and output. The function supports early stopping based on a threshold
 #     to prevent unnecessary computations if the activation change becomes negligible.
 
 #     Args:
 #         model: A PyTorch model with `activations`, `sensory_indices`, and `threshold` attributes.
-#         selected_neurons_per_layer (Dict[int, List[int]]): A dictionary mapping from layer indices to lists of neuron indices
+#         neurons_to_activate (Dict[int, List[int]]): A dictionary mapping from layer indices to lists of neuron indices
 #             whose activations are to be maximized.
 #         input_tensor (torch.Tensor, optional): The initial tensor to optimize. If None, a random tensor is created.
 #             Defaults to None.
 #         num_iterations (int, optional): The number of iterations to run the optimization for. Defaults to 300.
 #         learning_rate (float, optional): The learning rate for the optimizer. Defaults to 0.01.
 #         in_regularisation_lambda (float, optional): The regularization coefficient. Defaults to 0.4.
 #         custom_in_regularisation (Callable[[torch.Tensor], torch.Tensor], optional): A function that applies custom
@@ -512,17 +528,17 @@
 #             snapshot = np.where(snapshot >= model.threshold,
 #                                 snapshot, 0)  # Thresholded ReLU
 #             # Limit the range between 0 and 1
 #             snapshot = np.tanh(snapshot)
 #             input_snapshots.append(snapshot)
 
 #         activation_loss = torch.tensor(0.0, device=input_tensor.device)
-#         # Check if the model has an 'activations' attribute and the selected_neurons_per_layer is not empty
-#         if hasattr(model, 'activations') and selected_neurons_per_layer:
-#             for layer_index, neuron_indices in selected_neurons_per_layer.items():
+#         # Check if the model has an 'activations' attribute and the neurons_to_activate is not empty
+#         if hasattr(model, 'activations') and neurons_to_activate:
+#             for layer_index, neuron_indices in neurons_to_activate.items():
 #                 # first transform the neuron_indices to indices of non_sensory neurons only
 #                 non_sensory_only_indices = [
 #                     all_to_nonsensory_map[idx] for idx in neuron_indices]
 #                 # Ensure layer index is valid
 #                 if layer_index < model.activations.shape[1]:
 #                     # Get activations for this layer
 #                     layer_activations = model.activations[:, layer_index]
@@ -580,15 +596,15 @@
     Generates a dataframe representing the paths in a layered plot, filtering by activation and connectivity thresholds.
 
     This function takes the direct connectivity matrix (inprop), optimal input neuron activity, output neuron activity, indices for sensory neurons, and mapping between input and output indices to groups. It generates a dataframe that represents the paths through the network layers.
 
     Args:
         inprop (scipy.sparse matrix or numpy.ndarray): Matrix representing the synaptic strengths
             between neurons, can be dense or sparse. Presynaptic is in the rows, postsynaptic in the columns.
-        opt_in (numpy.ndarray): A 2D array representing optimal input to the network.
+        opt_in (numpy.ndarray): A 2D array representing optimal input to the network. Neurons are in the rows, timepoints in the columns. Only the first timepoint is used, since `out` is expected to have activity of all neurons, including input neurons.
         out (numpy.ndarray): A 2D array representing the output from the network. The second dimension represents timepoints.
         sensory_indices (list of int): A list of indices corresponding to sensory neurons in `inprop`.
         inidx_mapping (dict, optional): A dictionary mapping indices in `inprop` to new indices. If None, indices are not remapped.
                                        Defaults to None.
         outidx_mapping (dict, optional): A dictionary mapping indices in `out` to new indices. If None, `inidx_mapping` is used for
                                          mapping. Defaults to None.
         activation_threshold (float, optional): A threshold value for activation. Neurons with activations below this threshold are
```

### Comparing `connectome_interpreter-1.6.5/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.7.0/connectome_interpreter/compress_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     sum_matrix = matrices[0].copy()
     for i in range(1, n):
         sum_matrix += matrices[i]
 
     return sum_matrix
 
 
-def result_summary(stepsn, inidx, outidx, inidx_map=None, outidx_map=None, display_output=True, sort_by_column=None, pre_in_column=False, display_threshold=0):
+def result_summary(stepsn, inidx, outidx, inidx_map=None, outidx_map=None, display_output=True, sort_by_column=None, pre_in_column=False, display_threshold=0, include_undefined_groups=False):
     """
     Generates a summary of connections between different types of neurons, 
     represented by their input and output indexes. The function calculates 
     the total synaptic input from presynaptic neuron groups to an average neuron in each 
     postsynaptic neuron group.
 
     Args:
@@ -220,14 +220,15 @@
         inidx_map (dict, optional): Mapping from indices to neuron groups for the input neurons. Defaults to None, in which case neurons are not grouped. 
         outidx_map (dict, optional): Mapping from indices to neuron groups for the output neurons.
             Defaults to None, in which case it is set to be the same as inidx_map.
         display_output (bool, optional): Whether to display the output in a coloured dataframe. Defaults to True.
         sort_by_column (str or list, optional): the column name(s) to sort the result by. If none is provided, then sort by the first column. 
         pre_in_column (bool, optional): Whether to have the presynaptic neuron groups as columns. Defaults to False (pre in rows, post in columns).
         display_threshold (float, optional): The threshold for displaying the output. Defaults to 0.
+        include_undefined_groups (bool, optional): Whether to include undefined groups in the output. Defaults to False.
 
     Returns:
         pd.DataFrame: A dataframe representing the summed synaptic input from presynaptic neuron groups 
             to an average neuron in each postsynaptic neuron group. This dataframe is always returned, regardless of the
             value of display_output.
 
     Displays:
@@ -243,19 +244,27 @@
     outidx = to_nparray(outidx)
 
     if issparse(stepsn):
         matrix = stepsn[:, outidx][inidx, :].toarray()
     else:
         matrix = stepsn[inidx, :][:, outidx]
 
+    if include_undefined_groups:
+        # fill the nan values in inidx_map (e.g. 17726: nan) and outidx_map with 'undefined'
+        inidx_map = {k: v if pd.notna(
+            v) else 'undefined' for k, v in inidx_map.items()}
+        outidx_map = {k: v if pd.notna(
+            v) else 'undefined' for k, v in outidx_map.items()}
+
     # Create the dataframe
     df = pd.DataFrame(data=matrix,
                       # choose what to group by here
-                      index=[inidx_map[key] for key in inidx],
-                      columns=[outidx_map[key] for key in outidx])
+                      # if idx is mapped to root_id, if root_id is kept as int64, the root_ids seem a bit messed up
+                      index=[str(inidx_map[key]) for key in inidx],
+                      columns=[str(outidx_map[key]) for key in outidx])
 
     # Sum across rows: presynaptic neuron is in the rows
     # summing across neurons of the same type: total amount of input from that type for the postsynaptic neuron
     summed_df = df.groupby(df.index).sum()
 
     # Average across columns and transpose back
     # averaging across columns of the same type:
```

### Comparing `connectome_interpreter-1.6.5/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.7.0/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.5/connectome_interpreter/utils.py` & `connectome_interpreter-1.7.0/connectome_interpreter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,18 +394,19 @@
         The function relies on the Neuroglancer library for layer creation and scene manipulation.
     """
 
     try:
         import nglscenes as ngl
     except ImportError:
         raise ImportError(
-            "To use this function, please install the package by running 'pip3 install git+https://github.com/schlegelp/nglscenes@main]'")
+            "To use this function, please install the package by running 'pip3 install git+https://github.com/schlegelp/nglscenes@main'")
 
     # define a scene if not given:
     if scene == None:
+        no_scene_provided = True
         # Initialize a scene
         scene = ngl.Scene()
         scene['layout'] = '3d'
         scene['position'] = [527216.1875, 208847.125, 84774.0625]
         scene['projectionScale'] = 400000
         scene['dimensions'] = {"x": [1e-9, "m"],
                                "y": [1e-9, "m"], "z": [1e-9, "m"]}
@@ -414,39 +415,38 @@
         fafb_layer = ngl.SegmentationLayer(source='precomputed://https://spine.itanna.io/files/eric/jfrc_mesh_test',
                                            name='jfrc_mesh_test1')
         fafb_layer['segments'] = ['1']
         fafb_layer['objectAlpha'] = 0.17
         fafb_layer['selectedAlpha'] = 0.55
         fafb_layer['segmentColors'] = {'1': '#cacdd8'}
         fafb_layer['colorSeed'] = 778769298
-        scene.add_layers(fafb_layer)
 
         # and the neuropil layer with names
         np_layer = ngl.SegmentationLayer(source='precomputed://gs://neuroglancer-fafb-data/elmr-data/FAFBNP.surf/mesh#type=mesh',
                                          name='neuropil_regions_surface_named')
         np_layer['segments'] = [str(num) for num in range(0, 79)]
         np_layer['visible'] = False
         np_layer['objectAlpha'] = 0.17
-        scene.add_layers(np_layer)
 
     # Define a list of colors optimized for human perception on a dark background
     colors = ['#ff6b6b', '#f06595', '#cc5de8', '#845ef7', '#5c7cfa', '#339af0', '#22b8cf', '#20c997', '#51cf66', '#94d82d', '#fcc419', '#4ecdc4',
               '#ffe66d', '#7bed9f', '#a9def9', '#f694c1', '#c7f0bd', '#ffc5a1', '#ff8c94', '#ffaaa6', '#ffd3b5', '#a8e6cf', '#a6d0e4', '#c1beff', '#f5b0cb']
 
     # Normalize the values in the DataFrame
     if normalise_within_column:
         df_norm = (df - df.min()) / (df.max() - df.min())
     else:
         df_norm = (df - df.min().min()) / (df.max().max() - df.min().min())
 
     scene['layout'] = '3d'
 
-    source = 'precomputed://gs://flywire_v141_m783'
+    source = ['precomputed://gs://flywire_v141_m783',
+              'precomputed://https://flyem.mrc-lmb.cam.ac.uk/flyconnectome/dynann/flytable-info-783-all']
 
-    for column in df.columns:
+    for i, column in enumerate(df.columns):
         color = random.choice(colors)
         cmap = mcl.LinearSegmentedColormap.from_list(
             "custom_cmap", ["white", color])
 
         df_group = df_norm[[column]]
         if no_connection_invisible:
             df_group = df_group[df_group.iloc[:, 0] > 0]
@@ -455,32 +455,42 @@
 
         layer['segments'] = list(df_group.index.astype(str))
         layer['segmentColors'] = {
             # trick from Claud to make the colours more saturated
             str(root_id): mcl.to_hex(cmap(colour_saturation + (1-colour_saturation)*value.values[0]))
             for root_id, value in df_group.iterrows()
         }
+        # only the first layer is visible
+        if i == 0:
+            layer['visible'] = True
+        else:
+            layer['visible'] = False
+
         if include_postsynaptic_neuron:
             layer['segments'].append(str(df_group.columns[0]))
             layer['segmentColors'][str(df_group.columns[0])] = '#43A7FF'
 
         scene.add_layers(layer)
 
+    if no_scene_provided:
+        # add FAFB and NP layers at the end
+        scene.add_layers(fafb_layer)
+        scene.add_layers(np_layer)
+
     return scene.url
 
 
 def get_activations(array, global_indices, idx_map=None, top_n=None, threshold=None):
     """
-    Identifies the top activated neurons for each column in the array,
-    either by number (top n) or by a minimum activation threshold, or both.
+    Get activation for neurons (in rows) in `array` for each time step (in columns). Optionally group neurons by `idx_map`, and filter by `top_n` or `threshold`.
 
     Args:
         array (np.ndarray): 2D array of neuron activations, where rows represent neurons
             and columns represent different time steps.
-        global_indices (int, list, set, np.ndarray, pd.Series): Array of global neuron indices corresponding to the rows of the array.
+        global_indices (int, list, set, np.ndarray, pd.Series): Array of global neuron indices corresponding to keys in `idx_map`. 
         idx_map (dict, optional): Mapping from neuron index (`global_indices`) to neuron identifier. If not None, and if multiple neurons map to the same identifier, the activations are averaged. Defaults to None.
         top_n (int, optional): Number of top activations to return for each column. If None,
             all activations above the threshold are returned. Defaults to None.
         threshold (float, dict, optional): Minimum activation level to consider. If a dictionary is provided, the threshold for each column is specified by the column index. Defaults to None.
 
     Returns:
         dict: A dictionary where each key is a column index and each value is a nested dictionary
@@ -502,63 +512,63 @@
                            global_idx in enumerate(indices)}
 
     for col in range(array.shape[1]):
         # Determine which indices to use based on the 'sensory' flag
         # these are global indices in the all-to-all connectivity
 
         column_values = array[:, col]
+        local_indices = np.asarray(range(len(column_values)))
 
         # Filter activations by threshold if provided
         if threshold is not None:
             if isinstance(threshold, dict):
                 if col not in threshold:
                     thresh = 0
                 else:
                     thresh = threshold[col]
             else:
                 thresh = threshold
 
             if thresh > 0:
                 # these are local indices
-                filtered_indices = np.where(column_values >= thresh)[0]
-                # these are global indices
-                threshold_indices = indices[filtered_indices]
-            else:
-                threshold_indices = indices
-        else:
-            threshold_indices = indices
+                local_indices -= np.where(column_values < thresh)[0]
 
         # Sort the filtered activations
-        # these are the local indices corresponding to only sensory/non-sensory neurons, but not both
+        # these are the local indices
         sorted_indices = np.argsort(
             column_values)[-top_n:] if top_n is not None else np.argsort(column_values)
-        # these are global indices
-        topn_indices = indices[sorted_indices]
 
-        selected = np.intersect1d(threshold_indices, topn_indices)
+        # get intersection of sorted_indices and local_indices, in the same order as sorted_indices
+        selected_local = [
+            index for index in sorted_indices if index in local_indices]
+        selected_global = indices[selected_local]
 
         # Build the result dictionary
         if idx_map is None:
             result[col] = {idx: column_values[global_to_local_map[idx]]
-                           for idx in selected}
+                           for idx in selected_global}
         else:
-            # initialise a zero dict
-            result[col] = {idx_map[idx]: [] for idx in selected}
-            # calculate the average
-            for idx in selected:
+            # initialise a dict of empty lists
+            result[col] = {idx_map[idx]: [] for idx in selected_global}
+
+            for idx in selected_global:
                 result[col][idx_map[idx]].append(
                     column_values[global_to_local_map[idx]])
+            # grouped indices by idx_map
             new_indices = result[col].keys()
+            # calculate the average
             result[col] = {idx: np.mean(result[col][idx])
                            for idx in new_indices}
 
     return result
 
 
-def plot_layered_paths(path_df, figsize=(10, 8), priority_indices=None, sort_by_activation=False, fraction=0.03, pad=0.02):
+def plot_layered_paths(path_df, figsize=(10, 8), priority_indices=None, sort_by_activation=False,
+                       fraction=0.03, pad=0.02, weight_decimals=2,
+                       neuron_to_sign=None, sign_color_map={1: 'red', -1: 'blue'}):
     """
     Plots a directed graph of layered paths with optional node coloring based on activation values.
 
     This function creates a visualization of a directed graph with nodes placed in layers. Nodes can be optionally
     colored based on 'pre_activation' and 'post_activation' columns present in the dataframe. If these columns are
     missing, a default color is used for all nodes. The edges are weighted, and their labels represent the weight values.
 
@@ -571,14 +581,17 @@
                                     their activation values.
         figsize (tuple, optional): A tuple indicating the size of the matplotlib figure. Defaults to (10, 8).
         priority_indices (list, optional): A list of indices to prioritize when creating the layered positions. Nodes with these
                                     indices will be placed at the top of their respective layers. Defaults to None. 
         sort_by_activation (bool, optional): A flag to sort the nodes based on their activation values (after grouping by priority). Defaults to False.
         fraction (float, optional): The fraction of the figure width to use for the colorbar. Defaults to 0.03.
         pad (float, optional): The padding between the colorbar and the plot. Defaults to 0.02.
+        weight_decimals (int, optional): The number of decimal places to display for edge weights. Defaults to 2.
+        neuron_to_sign (dict, optional): A dictionary mapping neuron names (as they appear in path_df) to their signs (e.g. {'KCg-m': 1, 'Delta7': -1}). Defaults to None.
+        sign_color_map (dict, optional): A dictionary mapping neuron signs to colors. Defaults to red for excitatory, and blue for inhibitory. Edges are in lightgrey by default.
 
     Returns:
         None: This function does not return a value. It generates a plot using matplotlib.
 
     Note:
         If 'pre_layer' and 'post_layer' columns are not in the dataframe, they will be created within the function
         to uniquely identify the nodes based on their 'pre'/'post' values and 'layer'.
@@ -633,31 +646,44 @@
             G, dict(zip(path_df.pre_layer, path_df.pre_activation)), 'activation')
         nx.set_node_attributes(
             G, dict(zip(path_df.post_layer, path_df.post_activation)), 'activation')
 
         node_colors = [color_map(norm(G.nodes[node]['activation']))
                        for node in G.nodes()]
 
+    # Edge colors based on neuron signs
+    default_color = 'lightgrey'  # Default edge color
+
+    # specify edge colour based on pre-neuron sign, if available
+    edge_colors = []
+    for u, _ in G.edges():
+        pre_neuron = labels[u]
+        if neuron_to_sign and pre_neuron in neuron_to_sign:
+            edge_colors.append(sign_color_map.get(
+                neuron_to_sign[pre_neuron], default_color))
+        else:
+            edge_colors.append(default_color)
+
     # Plot the graph
-    fig, ax = plt.subplots(figsize=figsize)
+    _, ax = plt.subplots(figsize=figsize)
     if ('pre_activation' in path_df.columns) & ('post_activation' in path_df.columns):
         nx.draw(G, pos=positions,
                 labels=labels,
                 with_labels=True, node_size=100,
                 node_color=node_colors,
                 arrows=True, arrowstyle='-|>', arrowsize=10,
-                font_size=8, width=widths, edge_color='lightgrey', ax=ax)
+                font_size=8, width=widths, edge_color=edge_colors, ax=ax)
         plt.colorbar(plt.cm.ScalarMappable(
             norm=norm, cmap=color_map), ax=ax, label='Activation', fraction=fraction, pad=pad)
     else:
         nx.draw(G, pos=positions,
                 labels=labels,
                 with_labels=True, node_size=100,
-                node_color='lightblue', arrows=True, arrowstyle='-|>', arrowsize=10, font_size=8, width=widths, ax=ax)
+                node_color='lightblue', arrows=True, arrowstyle='-|>', arrowsize=10, font_size=8, width=widths, ax=ax, edge_color=edge_colors)
 
-    edge_labels = {(u, v): f'{data["weight"]:.2f}' for u,
+    edge_labels = {(u, v): f'{data["weight"]:.{weight_decimals}f}' for u,
                    v, data in G.edges(data=True)}
     nx.draw_networkx_edge_labels(G, pos=positions, edge_labels=edge_labels,
                                  #  font_color='red'
                                  ax=ax)
     ax.set_ylim(0, 1)
     plt.show()
```

### Comparing `connectome_interpreter-1.6.5/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.7.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.6.5
+Version: 1.7.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.6.5/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.7.0/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.5/setup.py` & `connectome_interpreter-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.6.5',
+    version='1.7.0',
     packages=find_packages(),
     install_requires=install_requires_list,
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
```

### Comparing `connectome_interpreter-1.6.5/tests/test_compress_paths.py` & `connectome_interpreter-1.7.0/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.5/tests/test_utils.py` & `connectome_interpreter-1.7.0/tests/test_utils.py`

 * *Files identical despite different names*

