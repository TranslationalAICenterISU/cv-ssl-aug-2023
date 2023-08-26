
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
	2. Speech
		1. Whisper
			1. https://huggingface.co/spaces/sanchit-gandhi/whisper-jax
3. **Novel Algorithms for enhancing AI**
	1. Self-supervised learning
		1. https://arxiv.org/pdf/2304.12210.pdf
	2. Neural Fields
		1. https://sites.google.com/berkeley.edu/nerf-tutorial
		2. https://arxiv.org/pdf/2111.11426.pdf
		3. https://arxiv.org/pdf/2210.00379.pdf
		4. https://neuralfields.cs.brown.edu/cvpr22.html

4. **Generative AI and its implications**
	1. Large Language Models
		1. https://cims.nyu.edu/~sbowman/eightthings.pdf
		2. https://arxiv.org/pdf/2303.12712.pdf
		3. https://sebastianraschka.com/blog/2023/llm-reading-list.html?s=31
	2. Transformers
		1. https://arxiv.org/abs/2302.07730
		2. https://www.youtube.com/playlist?list=PLoROMvodv4rNiJRchCzutFw5ItR_Z27CM
5. **Science in AI and AI in Science**
	1. Healthcare application
		1. https://huggingface.co/spaces/suppfunterpno/Heart-Failure-Death-Prediction
	2. Protein folding
		1. https://esmatlas.com/resources/fold/result?fasta_header=%3EHallucinated%20protein%20HALC1_878&sequence=MSGMKKLYEYTVTTLDEFLEKLKEFILNTSKDKIYKLTITNPKLIKDIGKAIAKAAEIADVDPKEIEEMIKAVEENELTKLVITIEQTDDKYVIKVELENEDGLVHSFEIYFKNKEEMEKFLELLEKLISKLSGS
	3. Physics informed neural networks
		1. https://docs.nvidia.com/deeplearning/modulus/modulus-sym/user_guide/theory/architectures.html#deeponet
		2. https://arxiv.org/pdf/2304.00567.pdf
		3. https://arxiv.org/pdf/2207.05748.pdf
		4. https://arxiv.org/pdf/2111.13587.pdf
		5. https://arxiv.org/pdf/2304.13799.pdf
		6. https://developer.nvidia.com/modulus?ncid=so-link-410285-vt25#cid=hpc03_so-link_en-us
6. **Trends in AI**
	1. https://www.capgemini.com/wp-content/uploads/2017/09/five_senses_pov.pdf
	2. https://aiindex.stanford.edu/wp-content/uploads/2021/11/2021-AI-Index-Report_Master.pdf
	3. https://hai.stanford.edu/sites/default/files/ai_index_2019_report.pdf
	4. https://aiindex.stanford.edu/wp-content/uploads/2023/04/HAI_AI-Index-Report_2023.pdf
