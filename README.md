# Efficient-and-Accurate-Scene-Text-Detector

Previous approaches for scene text detection have already achieved promising performances across various benchmarks. However, they usually fall short when dealing with challenging scenarios, even when equipped with deep neural network models, because the overall performance is determined by the interplay of multiple stages and components in the pipelines. In this work, we propose a simple yet powerful pipeline that yields fast and accurate text detection in natural scenes. The pipeline directly predicts words or text lines of arbitrary orientations and quadrilateral shapes in full images, eliminating unnecessary intermediate steps (e.g., candidate aggregation and word partitioning), with a single neural network. The simplicity of our pipeline allows concentrating efforts on designing loss functions and neural network architecture.



##Inference

python text_recognition.py --east  --image  --padding --min-confidenc --width --height

--image : The path to our input image.
--east : The EAST scene text detector model file path.
--min-confidence : Probability threshold to determine text. Optional with default=0.5 .
--width : Resized image width — must be multiple of 32. Optional with default=320 .
--height : Resized image height — must be multiple of 32. Optional with default=320 .
