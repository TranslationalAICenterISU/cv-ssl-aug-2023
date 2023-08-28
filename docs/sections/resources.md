
1. **Introduction**
	1. Tools for generating images using description
		1. [https://beta.dreamstudio.ai/generate](https://beta.dreamstudio.ai/generate)
		2. [https://huggingface.co/spaces/stabilityai/stable-diffusion](https://huggingface.co/spaces/stabilityai/stable-diffusion)
		3. [https://www.bing.com/create](https://www.bing.com/create)
	2. Research paper collection
		1. https://aman.ai/papers/
	3. Improving deep learning performance
		1. https://horace.io/brrr_intro.html
	4. Multi-model deep learning
		1. https://arxiv.org/pdf/2301.04856.pdf
	5. AI-based ppt generation
		1. https://slidesgpt.com/index.html
	6. Visualize your dreams
		1. https://beta.dreamstudio.ai/generate
	7. ChatGPT
		1. https://chat.openai.com/auth/login
2. **Multiple modalities of Data to enhance AI**
	1. Computer Vision
		1. -   Additional models for classification, pose estimation, depth estimation, and ReID are just gotten from paperswithcode rankings
		2. YOLOv8 is very good for exploring different computer vision tasks since it has detection, segmentation, classification, pose, and tracking (ByteTrack and BoT-SORT without ReID for now) implemented
		3. Object detection
			1. CNN-based
				1. Requires relatively little data (especially if pretrained with datasets such as COCO) fast inference
				2. YOLOv8 (still no actual paper)
					-   [https://github.com/ultralytics/ultralytics](https://github.com/ultralytics/ultralytics "https://github.com/ultralytics/ultralytics") 
					-   [https://blog.roboflow.com/whats-new-in-yolov8/](https://blog.roboflow.com/whats-new-in-yolov8/ "https://blog.roboflow.com/whats-new-in-yolov8/") 
				3. YOLOv6.3
					-   Situationally better than v8, but it isn't as user-friendly and doesn't have additional functionality (segmentation, classification, pose)
					- [https://arxiv.org/abs/2301.05586](https://arxiv.org/abs/2301.05586 "https://arxiv.org/abs/2301.05586") 
			2. Transformer-based detection
				1. Generally requires more data and has slower inference but can detect many more types of objects/classes
				2. DETR
					1. [https://github.com/facebookresearch/detr](https://github.com/facebookresearch/detr "https://github.com/facebookresearch/detr") 
					2. [https://arxiv.org/abs/2005.12872](https://arxiv.org/abs/2005.12872 "https://arxiv.org/abs/2005.12872") 
				3. Grounding DINO: SOTA Zero-Shot Objection Detection
					1. Can detect new classes with no additional training, one of their examples is a dog's tail
					2. [https://blog.roboflow.com/grounding-dino-zero-shot-object-detection/](https://blog.roboflow.com/grounding-dino-zero-shot-object-detection/ "https://blog.roboflow.com/grounding-dino-zero-shot-object-detection/")
					3. [https://arxiv.org/abs/2303.05499](https://arxiv.org/abs/2303.05499 "https://arxiv.org/abs/2303.05499") 
				4. DINO v2
					1. [https://ai.facebook.com/blog/dino-v2-computer-vision-self-supervised-learning/](https://ai.facebook.com/blog/dino-v2-computer-vision-self-supervised-learning/ "https://ai.facebook.com/blog/dino-v2-computer-vision-self-supervised-learning/") 
					2. [https://arxiv.org/abs/2304.07193](https://arxiv.org/abs/2304.07193 "https://arxiv.org/abs/2304.07193")
		4. Object segmentation
			1. YOLOv8 also has segmentation
				1. Segment anything
				2. [https://ai.facebook.com/blog/segment-anything-foundation-model-image-segmentation/](https://ai.facebook.com/blog/segment-anything-foundation-model-image-segmentation/ "https://ai.facebook.com/blog/segment-anything-foundation-model-image-segmentation/") 
				3. https://segment-anything.com/
				4. https://huggingface.co/spaces/curt-park/segment-anything-with-clip
		5. Classification
			1. YOLOv8 also has classification
			2. CoCa: Contrastive Captioners
				1. [https://arxiv.org/abs/2205.01917](https://arxiv.org/abs/2205.01917 "https://arxiv.org/abs/2205.01917")
		6. Pose estimation
			1. YOLOv8 also has pose
			2. ViTPose+
				1. [https://github.com/vitae-transformer/vitpose](https://github.com/vitae-transformer/vitpose "https://github.com/vitae-transformer/vitpose") 
				2. [https://arxiv.org/abs/2212.04246](https://arxiv.org/abs/2212.04246 "https://arxiv.org/abs/2212.04246") 
				3. [https://arxiv.org/abs/2204.12484](https://arxiv.org/abs/2204.12484 "https://arxiv.org/abs/2204.12484") 
		7. Tracking
			1. BoT-SORT
				1. [https://arxiv.org/abs/2206.14651](https://arxiv.org/abs/2206.14651 "https://arxiv.org/abs/2206.14651") 
			2. Deep OC-SORT
				1. Better than BoT-SORT in some metrics, and worse in others, but it also runs faster (good for edge devices where the lower fps of BoT-SORT can impact the motion model)
				2. [https://arxiv.org/abs/2302.11813](https://arxiv.org/abs/2302.11813 "https://arxiv.org/abs/2302.11813")
			3. Person ReID
			4. Fast-ReID: A Pytorch Toolbox for General Instance Re-identification
				1. [https://arxiv.org/abs/2006.02631](https://arxiv.org/abs/2006.02631 "https://arxiv.org/abs/2006.02631")
			5. DenseIL – Dense Interaction Learning for Video-based Person Re-identification 
				1. [https://arxiv.org/pdf/2103.09013v3.pdf](https://arxiv.org/pdf/2103.09013v3.pdf "https://arxiv.org/pdf/2103.09013v3.pdf")
		8. Depth estimation
			1. HiMODE
				1. [https://arxiv.org/pdf/2204.05007v1.pdf](https://arxiv.org/pdf/2204.05007v1.pdf "https://arxiv.org/pdf/2204.05007v1.pdf")
			2. FreDSNet
				1. [https://github.com/sbrunoberenguel/fredsnet](https://github.com/sbrunoberenguel/fredsnet "https://github.com/sbrunoberenguel/fredsnet")
				2. [https://arxiv.org/pdf/2210.01595v1.pdf](https://arxiv.org/pdf/2210.01595v1.pdf "https://arxiv.org/pdf/2210.01595v1.pdf")
		9. Many more notebooks for various computer vision tasks
			1. Roboflow Notebooks
				1. [https://github.com/roboflow/notebooks](https://github.com/roboflow/notebooks)
			2. OpenVINO Notebooks
				1. [https://github.com/openvinotoolkit/openvino_notebooks](https://github.com/openvinotoolkit/openvino_notebooks)
			3. Microsoft Computer Vision Recipes
				1. [https://github.com/microsoft/computervision-recipes/tree/staging/scenarios](https://github.com/microsoft/computervision-recipes/tree/staging/scenarios)
		10. Lots of practice exercises
			1. Udacity's Computer Vision Nanodegree program
				1. [https://github.com/udacity/CVND_Exercises](https://github.com/udacity/CVND_Exercises)
3. **Novel Algorithms for enhancing AI**
	1. Self-supervised learning
		1. https://arxiv.org/pdf/2304.12210.pdf

