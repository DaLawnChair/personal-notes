---
annotation-target: prejohned/rtdetr2.pdf
---


>%%
>```annotation-json
>{"created":"2025-02-16T19:11:33.776Z","text":"Why RT-DETR was good:\n* efficeint hybrid encoder compared to DETR transformers\n* decouled intra-scale interaction and cross-scale fusion of multi-scale features\n* uncertainy-minimal query selection, initiallizing the queries to the encoder with ones that are sure to be high quality\n* multiple detector sizes that can be swapped without retraining","updated":"2025-02-16T19:11:33.776Z","document":{"title":"","link":[{"href":"urn:x-pdf:f21979997608cd9b05205d9e17ad060c"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf"}],"documentFingerprint":"f21979997608cd9b05205d9e17ad060c"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","selector":[{"type":"TextPositionSelector","start":2127,"end":2732},{"type":"TextQuoteSelector","exact":"RT-DETR proposes an efficient hybrid encoder to replace thevanilla Transformer encoder in DETR (Carion et al. [2020]), which significantly improves the inference speed by de-coupling the intra-scale interaction and cross-scale fusion of multi-scale features. To further improve the performance,RT-DETR proposes the uncertainty-minimal query selection, which provides high-quality initial queries to the decoderby explicitly optimizing the uncertainty. Moreover, RT-DETR provides a wide range of detector sizes and supportsflexible speed tuning to accommodate various real-time scenarios without retraining","prefix":"ency on the YOLO in this field. ","suffix":". RT-DETR represents a novel,end"}]}]}
>```
>%%
>*%%PREFIX%%ency on the YOLO in this field.%%HIGHLIGHT%% ==RT-DETR proposes an efficient hybrid encoder to replace thevanilla Transformer encoder in DETR (Carion et al. [2020]), which significantly improves the inference speed by de-coupling the intra-scale interaction and cross-scale fusion of multi-scale features. To further improve the performance,RT-DETR proposes the uncertainty-minimal query selection, which provides high-quality initial queries to the decoderby explicitly optimizing the uncertainty. Moreover, RT-DETR provides a wide range of detector sizes and supportsflexible speed tuning to accommodate various real-time scenarios without retraining== %%POSTFIX%%. RT-DETR represents a novel,end*
>%%LINK%%[[#^t32jpm3ag8o|show annotation]]
>%%COMMENT%%
>Why RT-DETR was good:
>* efficeint hybrid encoder compared to DETR transformers
>* decouled intra-scale interaction and cross-scale fusion of multi-scale features
>* uncertainy-minimal query selection, initiallizing the queries to the encoder with ones that are sure to be high quality
>* multiple detector sizes that can be swapped without retraining
>%%TAGS%%
>
^t32jpm3ag8o


>%%
>```annotation-json
>{"created":"2025-02-16T19:15:14.617Z","text":"what is new?\n* discrete sampling of points for features at different scales within th edeformable attention module\n* discrete sampling operattor replacing the grid_sample operator\n* better training strategy with dynmaic data augmentation and scale-adaptive huperameteres","updated":"2025-02-16T19:15:14.617Z","document":{"title":"","link":[{"href":"urn:x-pdf:f21979997608cd9b05205d9e17ad060c"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf"}],"documentFingerprint":"f21979997608cd9b05205d9e17ad060c"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","selector":[{"type":"TextPositionSelector","start":3158,"end":3829},{"type":"TextQuoteSelector","exact":"RT-DETRv2 suggests setting a distinctnumber of sampling points for features at different scales within the deformable attention module to achieve selectivemulti-scale feature extraction by the decoder. In the realm of enhancing practicality, RT-DETRv2 provides an optionaldiscrete sampling operator to replace the original grid_sample operator, which is specific to DETRs, thus eliminatingthe deployment constraints typically associated with detection Transformers. Furthermore, RT-DETRv2 optimizesthe training strategy, including dynamic data augmentation and scale-adaptive hyperparameters customization, withthe objective of improving performance without loss of speed","prefix":"nced performance. Specifically, ","suffix":". The results demonstrate that R"}]}]}
>```
>%%
>*%%PREFIX%%nced performance. Specifically,%%HIGHLIGHT%% ==RT-DETRv2 suggests setting a distinctnumber of sampling points for features at different scales within the deformable attention module to achieve selectivemulti-scale feature extraction by the decoder. In the realm of enhancing practicality, RT-DETRv2 provides an optionaldiscrete sampling operator to replace the original grid_sample operator, which is specific to DETRs, thus eliminatingthe deployment constraints typically associated with detection Transformers. Furthermore, RT-DETRv2 optimizesthe training strategy, including dynamic data augmentation and scale-adaptive hyperparameters customization, withthe objective of improving performance without loss of speed== %%POSTFIX%%. The results demonstrate that R*
>%%LINK%%[[#^04s4el2clzuf|show annotation]]
>%%COMMENT%%
>what is new?
>* discrete sampling of points for features at different scales within th edeformable attention module
>* discrete sampling operattor replacing the grid_sample operator
>* better training strategy with dynmaic data augmentation and scale-adaptive huperameteres
>%%TAGS%%
>
^04s4el2clzuf


>%%
>```annotation-json
>{"created":"2025-02-16T19:18:43.182Z","text":"previously this deformable attention module used the same # of sampled features for each scale, however here they want to sample based on the scale itself ","updated":"2025-02-16T19:18:43.182Z","document":{"title":"","link":[{"href":"urn:x-pdf:f21979997608cd9b05205d9e17ad060c"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf"}],"documentFingerprint":"f21979997608cd9b05205d9e17ad060c"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","selector":[{"type":"TextPositionSelector","start":4643,"end":4961},{"type":"TextQuoteSelector","exact":"We argue that this constraint ignores the intrinsic differences in features at different scales and limitsthe feature extraction capability of the deformable attention module. Therefore, we propose to set distinct numbers ofsampling points for different scales to achieve more flexible and efficient feature extraction","prefix":"f sampling pointsat each scale. ","suffix":".Discrete sampling. To improve t"}]}]}
>```
>%%
>*%%PREFIX%%f sampling pointsat each scale.%%HIGHLIGHT%% ==We argue that this constraint ignores the intrinsic differences in features at different scales and limitsthe feature extraction capability of the deformable attention module. Therefore, we propose to set distinct numbers ofsampling points for different scales to achieve more flexible and efficient feature extraction== %%POSTFIX%%.Discrete sampling. To improve t*
>%%LINK%%[[#^mvm3g7yawl|show annotation]]
>%%COMMENT%%
>previously this deformable attention module used the same # of sampled features for each scale, however here they want to sample based on the scale itself 
>%%TAGS%%
>
^mvm3g7yawl


>%%
>```annotation-json
>{"created":"2025-02-16T19:20:42.685Z","text":"better deployability with this discrte_sample operator over the grid_sample operator, which is limited in inferencing applications. Uses the best of both worlds by switching it based on training or inferencing tasks","updated":"2025-02-16T19:20:42.685Z","document":{"title":"","link":[{"href":"urn:x-pdf:f21979997608cd9b05205d9e17ad060c"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf"}],"documentFingerprint":"f21979997608cd9b05205d9e17ad060c"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","selector":[{"type":"TextPositionSelector","start":5634,"end":5834},{"type":"TextQuoteSelector","exact":"we first employ the grid_sample operator for training and then replace it with the discrete_sample operator forfine-tuning. For inference and deployment, the model employs the discrete_sample operator","prefix":"e sampling offsets. In practice,","suffix":".2.2 Training SchemeDynamic data"}]}]}
>```
>%%
>*%%PREFIX%%e sampling offsets. In practice,%%HIGHLIGHT%% ==we first employ the grid_sample operator for training and then replace it with the discrete_sample operator forfine-tuning. For inference and deployment, the model employs the discrete_sample operator== %%POSTFIX%%.2.2 Training SchemeDynamic data*
>%%LINK%%[[#^mm02pc463li|show annotation]]
>%%COMMENT%%
>better deployability with this discrte_sample operator over the grid_sample operator, which is limited in inferencing applications. Uses the best of both worlds by switching it based on training or inferencing tasks
>%%TAGS%%
>
^mm02pc463li


>%%
>```annotation-json
>{"created":"2025-02-16T19:22:51.747Z","text":"basically has the hyparamteres built in to the model to change model specific parameters, here they denote learning rate as one of them depending on if you use the resnet50/101 backbone","updated":"2025-02-16T19:22:51.747Z","document":{"title":"","link":[{"href":"urn:x-pdf:f21979997608cd9b05205d9e17ad060c"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf"}],"documentFingerprint":"f21979997608cd9b05205d9e17ad060c"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/rtdetr2.pdf","selector":[{"type":"TextPositionSelector","start":6704,"end":7015},{"type":"TextQuoteSelector","exact":"Considering that the pre-trained backbone forlight detector (e.g., ResNet18 (He et al. [2016])) has lower feature quality, we increase its learning rate. On thecontrary, the pre-trained backbone with large detector (e.g., ResNet101 (He et al. [2016])) has higher feature qualityand we decrease its learning rate","prefix":"tomization for scaled RT-DETRs. ","suffix":".3 Experiment3.1 Implementation "}]}]}
>```
>%%
>*%%PREFIX%%tomization for scaled RT-DETRs.%%HIGHLIGHT%% ==Considering that the pre-trained backbone forlight detector (e.g., ResNet18 (He et al. [2016])) has lower feature quality, we increase its learning rate. On thecontrary, the pre-trained backbone with large detector (e.g., ResNet101 (He et al. [2016])) has higher feature qualityand we decrease its learning rate== %%POSTFIX%%.3 Experiment3.1 Implementation*
>%%LINK%%[[#^pyhbv8snr6b|show annotation]]
>%%COMMENT%%
>basically has the hyparamteres built in to the model to change model specific parameters, here they denote learning rate as one of them depending on if you use the resnet50/101 backbone
>%%TAGS%%
>
^pyhbv8snr6b
