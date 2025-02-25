---
annotation-target: prejohned/dfine.pdf
---


>%%
>```annotation-json
>{"created":"2025-02-16T03:44:36.070Z","text":"paper: https://arxiv.org/pdf/2407.17140","updated":"2025-02-16T03:44:36.070Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":0,"end":80},{"type":"TextQuoteSelector","exact":"D-FINE: REDEFINE REGRESSION TASK IN DETRS ASFINE-GRAINED DISTRIBUTION REFINEMENT","prefix":"th50%75%100%125%150%200%300%400%","suffix":"Yansong Peng1, Hebei Li1, Peixi "}]}]}
>```
>%%
>*%%PREFIX%%th50%75%100%125%150%200%300%400%%%HIGHLIGHT%% ==D-FINE: REDEFINE REGRESSION TASK IN DETRS ASFINE-GRAINED DISTRIBUTION REFINEMENT== %%POSTFIX%%Yansong Peng1, Hebei Li1, Peixi*
>%%LINK%%[[#^bnfavoeql1w|show annotation]]
>%%COMMENT%%
>paper: https://arxiv.org/pdf/2407.17140
>%%TAGS%%
>
^bnfavoeql1w


>%%
>```annotation-json
>{"created":"2025-02-16T20:56:49.433Z","text":"Problem status:\n* detectors predict bbox for regressed fixed coordinates, where edges are treated as values by Dirac delta distributions. This fails for localization uncertanity.\n* models are limited to use L1 and IoU loss, which aren't sufficient for adjusting each edge indeendently.\n* slow convergence and is sensitive to coordinate changes\n* other approaches rely n anchors, ie GFocal\n* Limited computation for real-time detectors. Knowledge distillation can be used, but are inefficient \n* local distillation is better for detection, but is challenging for anchor free detectors and training intensive","updated":"2025-02-16T20:56:49.433Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":3444,"end":4999},{"type":"TextQuoteSelector","exact":"Most detectors predict bounding boxes by regressing fixed coordinates, treating edgesas precise values modeled by Dirac delta distributions (Liu et al., 2016; Ren et al., 2015; Tian et al.,2019; Lyu et al., 2022). While straightforward, this approach fails to model localization uncertainty.Consequently, models are constrained to use L1 loss and IoU loss, which provide insufficient guid-ance for adjusting each edge independently (Girshick, 2015). This makes the optimization processsensitive to small coordinate changes, leading to slow convergence and suboptimal performance.Although methods like GFocal (Li et al., 2020; 2021) address uncertainty through probability dis-tributions, they remain limited by anchor dependency, coarse localization, and lack of iterative re-finement. Another challenge lies in maximizing the efficiency of real-time detectors, which areconstrained by limited computation and parameter budgets to maintain speed. Knowledge distilla-tion (KD) is a promising solution, transferring knowledge from larger teachers to smaller studentsto improve performance without increasing costs (Hinton et al., 2015). However, traditional KDmethods like Logit Mimicking and Feature Imitation have proven inefficient for detection tasks andcan even cause performance drops in state-of-the-art models (Zheng et al., 2022). In contrast, local-ization distillation (LD) has shown better results for detection. Nevertheless, integrating LD remainschallenging due to its substantial training overhead and incompatibility with anchor-free detect","prefix":"tion of bounding boxregression. ","suffix":"ors.To address these issues, we "}]}]}
>```
>%%
>*%%PREFIX%%tion of bounding boxregression.%%HIGHLIGHT%% ==Most detectors predict bounding boxes by regressing fixed coordinates, treating edgesas precise values modeled by Dirac delta distributions (Liu et al., 2016; Ren et al., 2015; Tian et al.,2019; Lyu et al., 2022). While straightforward, this approach fails to model localization uncertainty.Consequently, models are constrained to use L1 loss and IoU loss, which provide insufficient guid-ance for adjusting each edge independently (Girshick, 2015). This makes the optimization processsensitive to small coordinate changes, leading to slow convergence and suboptimal performance.Although methods like GFocal (Li et al., 2020; 2021) address uncertainty through probability dis-tributions, they remain limited by anchor dependency, coarse localization, and lack of iterative re-finement. Another challenge lies in maximizing the efficiency of real-time detectors, which areconstrained by limited computation and parameter budgets to maintain speed. Knowledge distilla-tion (KD) is a promising solution, transferring knowledge from larger teachers to smaller studentsto improve performance without increasing costs (Hinton et al., 2015). However, traditional KDmethods like Logit Mimicking and Feature Imitation have proven inefficient for detection tasks andcan even cause performance drops in state-of-the-art models (Zheng et al., 2022). In contrast, local-ization distillation (LD) has shown better results for detection. Nevertheless, integrating LD remainschallenging due to its substantial training overhead and incompatibility with anchor-free detect== %%POSTFIX%%ors.To address these issues, we*
>%%LINK%%[[#^urgqmhknro|show annotation]]
>%%COMMENT%%
>Problem status:
>* detectors predict bbox for regressed fixed coordinates, where edges are treated as values by Dirac delta distributions. This fails for localization uncertanity.
>* models are limited to use L1 and IoU loss, which aren't sufficient for adjusting each edge indeendently.
>* slow convergence and is sensitive to coordinate changes
>* other approaches rely n anchors, ie GFocal
>* Limited computation for real-time detectors. Knowledge distillation can be used, but are inefficient 
>* local distillation is better for detection, but is challenging for anchor free detectors and training intensive
>%%TAGS%%
>
^urgqmhknro


>%%
>```annotation-json
>{"created":"2025-02-16T21:03:36.927Z","updated":"2025-02-16T21:03:36.927Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":5395,"end":5754},{"type":"TextQuoteSelector","exact":" Fine-grained Distribution Refinement (FDR) to transform bounding box regression from predictingfixed coordinates to modeling probability distributions, providing a more fine-grained intermediaterepresentation. FDR refines these distributions iteratively in a residual manner, allowing for progres-sively finer adjustments and improving localization precision","prefix":"less training cost. We introduce","suffix":". Recognizing that deeper layers"}]}]}
>```
>%%
>*%%PREFIX%%less training cost. We introduce%%HIGHLIGHT%% ==Fine-grained Distribution Refinement (FDR) to transform bounding box regression from predictingfixed coordinates to modeling probability distributions, providing a more fine-grained intermediaterepresentation. FDR refines these distributions iteratively in a residual manner, allowing for progres-sively finer adjustments and improving localization precision== %%POSTFIX%%. Recognizing that deeper layers*
>%%LINK%%[[#^oi3hi3jrups|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^oi3hi3jrups


>%%
>```annotation-json
>{"created":"2025-02-16T21:03:55.234Z","updated":"2025-02-16T21:03:55.234Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":5975,"end":6281},{"type":"TextQuoteSelector","exact":"GO-LSDtransfers localization knowledge from deeper layers to shallower ones with negligible extra trainingcost. By aligning shallower layers’ predictions with refined outputs from later layers, the modellearns to produce better early adjustments, accelerating convergence and improving overall perfor-mance","prefix":"ion Self-Distillation (GO-LSD). ","suffix":". Furthermore, we streamline com"}]}]}
>```
>%%
>*%%PREFIX%%ion Self-Distillation (GO-LSD).%%HIGHLIGHT%% ==GO-LSDtransfers localization knowledge from deeper layers to shallower ones with negligible extra trainingcost. By aligning shallower layers’ predictions with refined outputs from later layers, the modellearns to produce better early adjustments, accelerating convergence and improving overall perfor-mance== %%POSTFIX%%. Furthermore, we streamline com*
>%%LINK%%[[#^5xrn9ooqpy2|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^5xrn9ooqpy2


>%%
>```annotation-json
>{"created":"2025-02-16T21:05:24.330Z","text":"Most rely on NMS, which transformers remove of and yolov10 does too, alllowing for quicker inferencing","updated":"2025-02-16T21:05:24.330Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":7667,"end":7706},{"type":"TextQuoteSelector","exact":"Real-Time / End-to-End Object Detectors","prefix":"ion in the field.22 RELATED WORK","suffix":". The YOLO series has led the wa"}]}]}
>```
>%%
>*%%PREFIX%%ion in the field.22 RELATED WORK%%HIGHLIGHT%% ==Real-Time / End-to-End Object Detectors== %%POSTFIX%%. The YOLO series has led the wa*
>%%LINK%%[[#^dqst4rzv6xh|show annotation]]
>%%COMMENT%%
>Most rely on NMS, which transformers remove of and yolov10 does too, alllowing for quicker inferencing
>%%TAGS%%
>
^dqst4rzv6xh


>%%
>```annotation-json
>{"created":"2025-02-16T21:06:31.859Z","text":"Guassian and discrete distributions of bboxes points are better than Dirac delta because of its precision, but limited scope currently due to anchor based networks","updated":"2025-02-16T21:06:31.859Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":9113,"end":9470},{"type":"TextQuoteSelector","exact":"Gaussian or discrete distributions to represent boundingboxes (Choi et al., 2019; Li et al., 2020; Qiu et al., 2020; Li et al., 2021), enhancing the modelingof uncertainty. However, these methods all rely on anchor-based frameworks, which limits theircompatibility with modern anchor-free detectors like YOLOX (Ge et al., 2021) and DETR (Carionet al., 2020)","prefix":"is, recent models have employed ","suffix":". Furthermore, their distributio"}]}]}
>```
>%%
>*%%PREFIX%%is, recent models have employed%%HIGHLIGHT%% ==Gaussian or discrete distributions to represent boundingboxes (Choi et al., 2019; Li et al., 2020; Qiu et al., 2020; Li et al., 2021), enhancing the modelingof uncertainty. However, these methods all rely on anchor-based frameworks, which limits theircompatibility with modern anchor-free detectors like YOLOX (Ge et al., 2021) and DETR (Carionet al., 2020)== %%POSTFIX%%. Furthermore, their distributio*
>%%LINK%%[[#^rxjbom152t|show annotation]]
>%%COMMENT%%
>Guassian and discrete distributions of bboxes points are better than Dirac delta because of its precision, but limited scope currently due to anchor based networks
>%%TAGS%%
>
^rxjbom152t


>%%
>```annotation-json
>{"created":"2025-02-16T21:08:29.822Z","text":"self-distillation","updated":"2025-02-16T21:08:29.822Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":10481,"end":10731},{"type":"TextQuoteSelector","exact":" Self-distillation (Zhang et al., 2019; 2021) is a spe-cial case of KD which enables earlier layers to learn from the model’s own refined outputs, requiringfar fewer additional training costs since there’s no need to separately train a teacher model.","prefix":"e effective for detection tasks.","suffix":"3 PRELIMINARIESBounding box regr"}]}]}
>```
>%%
>*%%PREFIX%%e effective for detection tasks.%%HIGHLIGHT%% ==Self-distillation (Zhang et al., 2019; 2021) is a spe-cial case of KD which enables earlier layers to learn from the model’s own refined outputs, requiringfar fewer additional training costs since there’s no need to separately train a teacher model.== %%POSTFIX%%3 PRELIMINARIESBounding box regr*
>%%LINK%%[[#^68cjoy8s412|show annotation]]
>%%COMMENT%%
>self-distillation
>%%TAGS%%
>
^68cjoy8s412


>%%
>```annotation-json
>{"created":"2025-02-16T21:12:14.571Z","text":"Dirac delta function for bbox regression is bad due to its precision","updated":"2025-02-16T21:12:14.571Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":10746,"end":11175},{"type":"TextQuoteSelector","exact":"Bounding box regression in object detection has traditionally relied on modeling Dirac delta distri-butions, either using centroid-based {x,y,w,h}or edge-distance {c,d}forms, where the distancesd = {t,b,l,r}are measured from the anchor point c = {xc,yc}. However, the Dirac delta assump-tion, which treats bounding box edges as precise and fixed, makes it difficult to model localizationuncertainty, especially in ambiguous cases","prefix":" a teacher model.3 PRELIMINARIES","suffix":". This rigid representation not "}]}]}
>```
>%%
>*%%PREFIX%%a teacher model.3 PRELIMINARIES%%HIGHLIGHT%% ==Bounding box regression in object detection has traditionally relied on modeling Dirac delta distri-butions, either using centroid-based {x,y,w,h}or edge-distance {c,d}forms, where the distancesd = {t,b,l,r}are measured from the anchor point c = {xc,yc}. However, the Dirac delta assump-tion, which treats bounding box edges as precise and fixed, makes it difficult to model localizationuncertainty, especially in ambiguous cases== %%POSTFIX%%. This rigid representation not*
>%%LINK%%[[#^1x8f3857fus|show annotation]]
>%%COMMENT%%
>Dirac delta function for bbox regression is bad due to its precision
>%%TAGS%%
>
^1x8f3857fus


>%%
>```annotation-json
>{"created":"2025-02-16T21:13:03.414Z","text":"why GFocal - regression on the bbox points ot the anchor center - is better, but not the best\n* anchor dependency\n* no iterative redefinement \n* coarse localization based on the chosen fixed distance bin intervals","updated":"2025-02-16T21:13:03.414Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":11939,"end":12203},{"type":"TextQuoteSelector","exact":"Anchor Dependency: Regression is tied to the anchor box center,limiting prediction diversity and compatibility with anchor-free frameworks. (2) No Iterative Refine-ment: Predictions are made in one shot without iterative refinements, reducing regression robustness","prefix":"egression approach persist: (1) ","suffix":".3(3) Coarse Localization: Fixed"}]}]}
>```
>%%
>*%%PREFIX%%egression approach persist: (1)%%HIGHLIGHT%% ==Anchor Dependency: Regression is tied to the anchor box center,limiting prediction diversity and compatibility with anchor-free frameworks. (2) No Iterative Refine-ment: Predictions are made in one shot without iterative refinements, reducing regression robustness== %%POSTFIX%%.3(3) Coarse Localization: Fixed*
>%%LINK%%[[#^6uvbwzsepkf|show annotation]]
>%%COMMENT%%
>why GFocal - regression on the bbox points ot the anchor center - is better, but not the best
>* anchor dependency
>* no iterative redefinement 
>* coarse localization based on the chosen fixed distance bin intervals
>%%TAGS%%
>
^6uvbwzsepkf


>%%
>```annotation-json
>{"created":"2025-02-16T21:16:14.500Z","updated":"2025-02-16T21:16:14.500Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":13332,"end":13884},{"type":"TextQuoteSelector","exact":"FDR iteratively optimizes probability distributions that act as corrections to the bounding boxpredictions, providing a more fine-grained intermediate representation. This approach captures andoptimizes the uncertainty of each edge independently. By leveraging the non-uniform weightingfunction, FDR allows for more precise and incremental adjustments at each decoder layer, improvinglocalization accuracy and reducing prediction errors. FDR operates within an anchor-free, end-to-end framework, enabling a more flexible and robust optimization process","prefix":"ters and training time cost.(1) ","suffix":".(2) GO-LSD distill localization"}]}]}
>```
>%%
>*%%PREFIX%%ters and training time cost.(1)%%HIGHLIGHT%% ==FDR iteratively optimizes probability distributions that act as corrections to the bounding boxpredictions, providing a more fine-grained intermediate representation. This approach captures andoptimizes the uncertainty of each edge independently. By leveraging the non-uniform weightingfunction, FDR allows for more precise and incremental adjustments at each decoder layer, improvinglocalization accuracy and reducing prediction errors. FDR operates within an anchor-free, end-to-end framework, enabling a more flexible and robust optimization process== %%POSTFIX%%.(2) GO-LSD distill localization*
>%%LINK%%[[#^s19uxedqqrs|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^s19uxedqqrs


>%%
>```annotation-json
>{"created":"2025-02-16T21:16:19.952Z","updated":"2025-02-16T21:16:19.952Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":13889,"end":14376},{"type":"TextQuoteSelector","exact":"GO-LSD distill localization knowledge from refined distributions into shallower layers. Astraining progresses, the final layer produces increasingly precise soft labels. Shallower layers aligntheir predictions with these labels through GO-LSD, leading to more accurate predictions. As early-stage predictions improve, the subsequent layers can focus on refining smaller residuals. This mutualreinforcement creates a synergistic effect, leading to progressively more accurate localization","prefix":"robust optimization process.(2) ","suffix":".To further enhance the efficien"}]}]}
>```
>%%
>*%%PREFIX%%robust optimization process.(2)%%HIGHLIGHT%% ==GO-LSD distill localization knowledge from refined distributions into shallower layers. Astraining progresses, the final layer produces increasingly precise soft labels. Shallower layers aligntheir predictions with these labels through GO-LSD, leading to more accurate predictions. As early-stage predictions improve, the subsequent layers can focus on refining smaller residuals. This mutualreinforcement creates a synergistic effect, leading to progressively more accurate localization== %%POSTFIX%%.To further enhance the efficien*
>%%LINK%%[[#^jir65kp40d|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^jir65kp40d


>%%
>```annotation-json
>{"created":"2025-02-16T21:22:22.120Z","text":"each edge of the bbox has its own distribution","updated":"2025-02-16T21:22:22.120Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":15196,"end":15586},{"type":"TextQuoteSelector","exact":"Each bounding box is associated with four distributions, one for each edge. The initial boundingboxes serve as reference boxes, while subsequent layers focus on refining them by adjusting distri-butions in a residual manner. The refined distributions are then applied to adjust the four edges ofthe corresponding initial bounding box, progressively improving its accuracy with each iteratio","prefix":"utput dimensions are different).","suffix":"n.Mathematically, let b0 = {x,y,"}]}]}
>```
>%%
>*%%PREFIX%%utput dimensions are different).%%HIGHLIGHT%% ==Each bounding box is associated with four distributions, one for each edge. The initial boundingboxes serve as reference boxes, while subsequent layers focus on refining them by adjusting distri-butions in a residual manner. The refined distributions are then applied to adjust the four edges ofthe corresponding initial bounding box, progressively improving its accuracy with each iteratio== %%POSTFIX%%n.Mathematically, let b0 = {x,y,*
>%%LINK%%[[#^xyd0zjy5xam|show annotation]]
>%%COMMENT%%
>each edge of the bbox has its own distribution
>%%TAGS%%
>
^xyd0zjy5xam


>%%
>```annotation-json
>{"created":"2025-02-16T21:23:44.599Z","text":"the distributions of each edge predicts a likelyhood of the offeset value for that edge. Combining these across all N indicies of the distrubition bins, we get the potential edge offset, which is scaled by a weighting factor and by the demension of the H and W of the intial box","updated":"2025-02-16T21:23:44.599Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":16213,"end":16687},{"type":"TextQuoteSelector","exact":" Each distribution predicts the likelihood of candidate offset values for the correspondingedge. These candidates are determined by the weighting function W(n), where n indexes the dis-crete bins out of N, with each bin corresponding to a potential edge offset. The weighted sum ofthe distributions produces the edge offsets. These edge offsets are then scaled by the height H andwidth W of the initial bounding box, ensuring the adjustments are proportional to the box size","prefix":"distributions, one foreach edge.","suffix":".4Refined Distributions Pr(n)Dec"}]}]}
>```
>%%
>*%%PREFIX%%distributions, one foreach edge.%%HIGHLIGHT%% ==Each distribution predicts the likelihood of candidate offset values for the correspondingedge. These candidates are determined by the weighting function W(n), where n indexes the dis-crete bins out of N, with each bin corresponding to a potential edge offset. The weighted sum ofthe distributions produces the edge offsets. These edge offsets are then scaled by the height H andwidth W of the initial bounding box, ensuring the adjustments are proportional to the box size== %%POSTFIX%%.4Refined Distributions Pr(n)Dec*
>%%LINK%%[[#^o49c4693wz|show annotation]]
>%%COMMENT%%
>the distributions of each edge predicts a likelyhood of the offeset value for that edge. Combining these across all N indicies of the distrubition bins, we get the potential edge offset, which is scaled by a weighting factor and by the demension of the H and W of the intial box
>%%TAGS%%
>
^o49c4693wz


>%%
>```annotation-json
>{"created":"2025-02-16T21:34:19.031Z","text":"kinda like MSE, good when close to correct, bad when not","updated":"2025-02-16T21:34:19.031Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":18116,"end":18472},{"type":"TextQuoteSelector","exact":"Asshown in Figure 2, the shape of W(n) ensures that when bounding box prediction is near accurate,small curvature in W(n) allows for finer adjustments. Conversely, if the bounding box predictionis far from accurate, the larger curvature near the edges and the sharp changes at the boundaries ofW(n) ensure sufficient flexibility for substantial corrections","prefix":" and curvature of the function. ","suffix":".To further improve the accuracy"}]}]}
>```
>%%
>*%%PREFIX%%and curvature of the function.%%HIGHLIGHT%% ==Asshown in Figure 2, the shape of W(n) ensures that when bounding box prediction is near accurate,small curvature in W(n) allows for finer adjustments. Conversely, if the bounding box predictionis far from accurate, the larger curvature near the edges and the sharp changes at the boundaries ofW(n) ensure sufficient flexibility for substantial corrections== %%POSTFIX%%.To further improve the accuracy*
>%%LINK%%[[#^c40q76dc6b6|show annotation]]
>%%COMMENT%%
>kinda like MSE, good when close to correct, bad when not
>%%TAGS%%
>
^c40q76dc6b6



>%%
>```annotation-json
>{"created":"2025-02-16T21:39:36.936Z","text":"* Starts off with Hungarian Matching to the predictions of each layer.\n* aggregates matching inidices of all layers into a set\n* These detections are the most accurate candidates predictions across the layers, so we ensure that these layers should be benefiting from the distillation.\n\n* classificaiton is still follows 1-to-1 matching, so no redundant boxes.\n\nIssues:\n* well-localized predictions because they exist in every layer, however they are low confidence ","updated":"2025-02-16T21:39:36.936Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":20631,"end":21661},{"type":"TextQuoteSelector","exact":"Thisprocess begins by applying Hungarian Matching (Carion et al., 2020) to the predictions from eachlayer, identifying the local bounding box matches at every stage of the model. To perform a globaloptimization, GO-LSD aggregates the matching indices from all layers into a unified union set.This union set combines the most accurate candidate predictions across layers, ensuring that theyall benefit from the distillation process. In addition to refining the global matches, GO-LSD alsooptimizes unmatched predictions during training to improve overall stability, leading to improvedoverall performance. Although the localization is optimized through this union set, the classificationtask still follows a one-to-one matching principle, ensuring that there are no redundant boxes. Thisstrict matching means that some predictions in the union set are well-localized but have low confi-dence scores. These low-confidence predictions often represent candidates with precise localization,which still need to be distilled effectively.","prefix":"r layers, as shown in Figure 3. ","suffix":"To address this, we introduce De"}]}]}
>```
>%%
>*%%PREFIX%%r layers, as shown in Figure 3.%%HIGHLIGHT%% ==Thisprocess begins by applying Hungarian Matching (Carion et al., 2020) to the predictions from eachlayer, identifying the local bounding box matches at every stage of the model. To perform a globaloptimization, GO-LSD aggregates the matching indices from all layers into a unified union set.This union set combines the most accurate candidate predictions across layers, ensuring that theyall benefit from the distillation process. In addition to refining the global matches, GO-LSD alsooptimizes unmatched predictions during training to improve overall stability, leading to improvedoverall performance. Although the localization is optimized through this union set, the classificationtask still follows a one-to-one matching principle, ensuring that there are no redundant boxes. Thisstrict matching means that some predictions in the union set are well-localized but have low confi-dence scores. These low-confidence predictions often represent candidates with precise localization,which still need to be distilled effectively.== %%POSTFIX%%To address this, we introduce De*
>%%LINK%%[[#^k51dzw60e2a|show annotation]]
>%%COMMENT%%
>* Starts off with Hungarian Matching to the predictions of each layer.
>* aggregates matching inidices of all layers into a set
>* These detections are the most accurate candidates predictions across the layers, so we ensure that these layers should be benefiting from the distillation.
>
>* classificaiton is still follows 1-to-1 matching, so no redundant boxes.
>
>Issues:
>* well-localized predictions because they exist in every layer, however they are low confidence 
>%%TAGS%%
>
^k51dzw60e2a


>%%
>```annotation-json
>{"created":"2025-02-16T21:39:57.875Z","text":"aims to solve the issue with the predictions existing in every layer by weighting the IoU and confidence","updated":"2025-02-16T21:39:57.875Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":21732,"end":21860},{"type":"TextQuoteSelector","exact":"which applies decoupledweighting strategies to ensure that high-IoU but low-confidence predictions are given appropriateweight. ","prefix":" Distillation Focal (DDF) Loss, ","suffix":"The DDF Loss also weights matche"}]}]}
>```
>%%
>*%%PREFIX%%Distillation Focal (DDF) Loss,%%HIGHLIGHT%% ==which applies decoupledweighting strategies to ensure that high-IoU but low-confidence predictions are given appropriateweight.== %%POSTFIX%%The DDF Loss also weights matche*
>%%LINK%%[[#^6s4d5dfd77c|show annotation]]
>%%COMMENT%%
>aims to solve the issue with the predictions existing in every layer by weighting the IoU and confidence
>%%TAGS%%
>
^6s4d5dfd77c



>%%
>```annotation-json
>{"created":"2025-02-16T21:45:02.190Z","text":"initial results, bettered by removing all decoder projection layers and then adding Target Gating layers","updated":"2025-02-16T21:45:02.190Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":29092,"end":29487},{"type":"TextQuoteSelector","exact":"Starting with the baseline metrics of 53.0% AP,32M parameters, 110 GFLOPs, and 9.25 ms latency, we first remove all the decoder projection lay-ers. This modification reduces GFLOPs to 97 and cuts the latency to 8.02 ms, although it decreasesAP to 52.4%. To address this drop, we introduce the Target Gating Layer, which recovers the AP to52.8% with only a marginal increase in computational cost","prefix":" our proposed D-FINE framework. ","suffix":".The Target Gating Layer is stra"}]}]}
>```
>%%
>*%%PREFIX%%our proposed D-FINE framework.%%HIGHLIGHT%% ==Starting with the baseline metrics of 53.0% AP,32M parameters, 110 GFLOPs, and 9.25 ms latency, we first remove all the decoder projection lay-ers. This modification reduces GFLOPs to 97 and cuts the latency to 8.02 ms, although it decreasesAP to 52.4%. To address this drop, we introduce the Target Gating Layer, which recovers the AP to52.8% with only a marginal increase in computational cost== %%POSTFIX%%.The Target Gating Layer is stra*
>%%LINK%%[[#^nfhe02dy688|show annotation]]
>%%COMMENT%%
>initial results, bettered by removing all decoder projection layers and then adding Target Gating layers
>%%TAGS%%
>
^nfhe02dy688


>%%
>```annotation-json
>{"created":"2025-02-16T21:47:31.840Z","updated":"2025-02-16T21:47:31.840Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":33345,"end":33503},{"type":"TextQuoteSelector","exact":"Increasing the number of distribution bins improves performance, with a maximum AP of 53.7%achieved at N = 32. Beyond N = 32, no significant gain is observed.","prefix":"ting localization precision.(2) ","suffix":" (3) The temperature T con-trols"}]}]}
>```
>%%
>*%%PREFIX%%ting localization precision.(2)%%HIGHLIGHT%% ==Increasing the number of distribution bins improves performance, with a maximum AP of 53.7%achieved at N = 32. Beyond N = 32, no significant gain is observed.== %%POSTFIX%%(3) The temperature T con-trols*
>%%LINK%%[[#^4cbyr44ry42|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^4cbyr44ry42


>%%
>```annotation-json
>{"created":"2025-02-16T21:48:14.997Z","text":"basically the GO-LSD is the best distillation method explored with the model and it is negleable training improvement, and can even be viewed as better since it doesn't require training a teacher","updated":"2025-02-16T21:48:14.997Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":33924,"end":33958},{"type":"TextQuoteSelector","exact":"COMPARISON OF DISTILLATION METHODS","prefix":"ved localization accuracy.5.4.3 ","suffix":"Section 5.4.1 compares different"}]}]}
>```
>%%
>*%%PREFIX%%ved localization accuracy.5.4.3%%HIGHLIGHT%% ==COMPARISON OF DISTILLATION METHODS== %%POSTFIX%%Section 5.4.1 compares different*
>%%LINK%%[[#^zmplad3vb9s|show annotation]]
>%%COMMENT%%
>basically the GO-LSD is the best distillation method explored with the model and it is negleable training improvement, and can even be viewed as better since it doesn't require training a teacher
>%%TAGS%%
>
^zmplad3vb9s


>%%
>```annotation-json
>{"created":"2025-02-16T21:50:08.833Z","text":"large and small models performance difference not being too large is concerning, and the authors point to the shallow decoder layers leading to worse final-layer predictions","updated":"2025-02-16T21:50:08.833Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":36372,"end":36777},{"type":"TextQuoteSelector","exact":"performance gap between lighterD-FINE models and other compact models remains small. One possible reason is that shallow de-coder layers may yield less accurate final-layer predictions, limiting the effectiveness of distillinglocalization knowledge into earlier layers. Addressing this challenge necessitates enhancing the lo-calization capabilities of lighter models without increasing inference latency.","prefix":"n and Future Work: However, the ","suffix":" Future research couldinvestigat"}]}]}
>```
>%%
>*%%PREFIX%%n and Future Work: However, the%%HIGHLIGHT%% ==performance gap between lighterD-FINE models and other compact models remains small. One possible reason is that shallow de-coder layers may yield less accurate final-layer predictions, limiting the effectiveness of distillinglocalization knowledge into earlier layers. Addressing this challenge necessitates enhancing the lo-calization capabilities of lighter models without increasing inference latency.== %%POSTFIX%%Future research couldinvestigat*
>%%LINK%%[[#^hdzis2kdyfl|show annotation]]
>%%COMMENT%%
>large and small models performance difference not being too large is concerning, and the authors point to the shallow decoder layers leading to worse final-layer predictions
>%%TAGS%%
>
^hdzis2kdyfl


>%%
>```annotation-json
>{"created":"2025-02-16T21:52:20.087Z","text":"images were resized down to 640x640","updated":"2025-02-16T21:52:20.087Z","document":{"title":"dfine.pdf","link":[{"href":"urn:x-pdf:6dc838646fde36278e19aa3358edced8"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf"}],"documentFingerprint":"6dc838646fde36278e19aa3358edced8"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/dfine.pdf","selector":[{"type":"TextPositionSelector","start":49754,"end":49877},{"type":"TextQuoteSelector","exact":"To further improve training efficiency, we resize all images with resolutionsexceeding 640 ×640 down to 640 ×640 beforehand","prefix":"exclud-ing the first 5k images. ","suffix":". We use the standard COCO2017 ("}]}]}
>```
>%%
>*%%PREFIX%%exclud-ing the first 5k images.%%HIGHLIGHT%% ==To further improve training efficiency, we resize all images with resolutionsexceeding 640 ×640 down to 640 ×640 beforehand== %%POSTFIX%%. We use the standard COCO2017 (*
>%%LINK%%[[#^73pnqth5o9j|show annotation]]
>%%COMMENT%%
>images were resized down to 640x640
>%%TAGS%%
>
^73pnqth5o9j
