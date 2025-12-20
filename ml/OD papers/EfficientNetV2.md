---
annotation-target: prejohned/efficientnetv2.pdf
---


>%%
>```annotation-json
>{"created":"2025-02-22T01:31:59.296Z","updated":"2025-02-22T01:31:59.296Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":3703,"end":3889},{"type":"TextQuoteSelector","exact":"Our study shows in EfficientNets: (1) trainingwith very large image sizes is slow; (2) depthwise convolu-tions are slow in early layers. (3) equally scaling up everystage is sub-optimal.","prefix":" bottlenecks in Effi-cientNets. ","suffix":" Based on these observations, we"}]}]}
>```
>%%
>*%%PREFIX%%bottlenecks in Effi-cientNets.%%HIGHLIGHT%% ==Our study shows in EfficientNets: (1) trainingwith very large image sizes is slow; (2) depthwise convolu-tions are slow in early layers. (3) equally scaling up everystage is sub-optimal.== %%POSTFIX%%Based on these observations, we*
>%%LINK%%[[#^3p9q8wlwps|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^3p9q8wlwps


>%%
>```annotation-json
>{"created":"2025-02-22T01:32:54.956Z","text":"The approach is progressive learning, where the model starts off with training on small image sizes and weak regularization settings (ie for droput and data augmentation) that progressively gets image size and regularization get larger/stronger as epochs go by","updated":"2025-02-22T01:32:54.956Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":4614,"end":5239},{"type":"TextQuoteSelector","exact":"We argue that keeping the same regular-ization for different image sizes is not ideal: for the samenetwork, small image size leads to small network capac-ity and thus requires weak regularization; vice versa, largeimage size requires stronger regularization to combat overfit-ting (see Section 4.1). Based on this insight, we propose animproved method of progressive learning: in the early train-ing epochs, we train the network with small image size andweak regularization (e.g., dropout and data augmentation),then we gradually increase image size and add stronger reg-ularization. Built upon progressive resizing (Howard, ","prefix":"zes, causing adrop in accuracy. ","suffix":"2018),but by dynamically adjusti"}]}]}
>```
>%%
>*%%PREFIX%%zes, causing adrop in accuracy.%%HIGHLIGHT%% ==We argue that keeping the same regular-ization for different image sizes is not ideal: for the samenetwork, small image size leads to small network capac-ity and thus requires weak regularization; vice versa, largeimage size requires stronger regularization to combat overfit-ting (see Section 4.1). Based on this insight, we propose animproved method of progressive learning: in the early train-ing epochs, we train the network with small image size andweak regularization (e.g., dropout and data augmentation),then we gradually increase image size and add stronger reg-ularization. Built upon progressive resizing (Howard,== %%POSTFIX%%2018),but by dynamically adjusti*
>%%LINK%%[[#^jd7ll1fbo1k|show annotation]]
>%%COMMENT%%
>The approach is progressive learning, where the model starts off with training on small image sizes and weak regularization settings (ie for droput and data augmentation) that progressively gets image size and regularization get larger/stronger as epochs go by
>%%TAGS%%
>
^jd7ll1fbo1k


>%%
>```annotation-json
>{"created":"2025-02-22T01:41:02.225Z","text":"goals of the first efficientnet was to have a fast training model, though it came with a cost of paramters","updated":"2025-02-22T01:41:02.225Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":9630,"end":9996},{"type":"TextQuoteSelector","exact":" It leveragesNAS to search for the baseline EfficientNet-B0 that hasbetter trade-off on accuracy and FLOPs. The baseline modelis then scaled up with a compound scaling strategy to obtaina family of models B1-B7. While recent works have claimedlarge gains on training or inference speed, they are oftenworse than EfficientNet in terms of parameters and FLOPsefficienc","prefix":" FLOPs and parameter efficiency.","suffix":"y (Table 1). In this paper, we a"}]}]}
>```
>%%
>*%%PREFIX%%FLOPs and parameter efficiency.%%HIGHLIGHT%% ==It leveragesNAS to search for the baseline EfficientNet-B0 that hasbetter trade-off on accuracy and FLOPs. The baseline modelis then scaled up with a compound scaling strategy to obtaina family of models B1-B7. While recent works have claimedlarge gains on training or inference speed, they are oftenworse than EfficientNet in terms of parameters and FLOPsefficienc== %%POSTFIX%%y (Table 1). In this paper, we a*
>%%LINK%%[[#^lawpksuhgyq|show annotation]]
>%%COMMENT%%
>goals of the first efficientnet was to have a fast training model, though it came with a cost of paramters
>%%TAGS%%
>
^lawpksuhgyq


>%%
>```annotation-json
>{"created":"2025-02-22T01:42:38.744Z","text":"progressive resizing is 2.2x faster in training and leads to better slightly accuracy","updated":"2025-02-22T01:42:38.744Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":10991,"end":11338},{"type":"TextQuoteSelector","exact":"smaller image size leads to less computations and enableslarge batch size, and thus improves training speed by upto 2.2x. Notably, as pointed out in (Touvron et al., 2020;Brock et al., 2021), using smaller image size for trainingalso leads to slightly better accuracy. But unlike (Touvronet al., 2019), we do not finetune any layers after training","prefix":" inference. As shown in Table 2,","suffix":".Table 2. EfficientNet-B6 accura"}]}]}
>```
>%%
>*%%PREFIX%%inference. As shown in Table 2,%%HIGHLIGHT%% ==smaller image size leads to less computations and enableslarge batch size, and thus improves training speed by upto 2.2x. Notably, as pointed out in (Touvron et al., 2020;Brock et al., 2021), using smaller image size for trainingalso leads to slightly better accuracy. But unlike (Touvronet al., 2019), we do not finetune any layers after training== %%POSTFIX%%.Table 2. EfficientNet-B6 accura*
>%%LINK%%[[#^xb4de0mb26m|show annotation]]
>%%COMMENT%%
>progressive resizing is 2.2x faster in training and leads to better slightly accuracy
>%%TAGS%%
>
^xb4de0mb26m


>%%
>```annotation-json
>{"created":"2025-02-22T01:44:30.309Z","text":"why depthwise convolutions \n+ fewer paramters\n- cannot be utilized fully on accelerators","updated":"2025-02-22T01:44:30.309Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":11916,"end":12051},{"type":"TextQuoteSelector","exact":"Depthwise convolutions have fewerparameters and FLOPs than regular convolutions, but theyoften cannot fully utilize modern accelerators","prefix":"se convolu-tions (Sifre, 2014). ","suffix":". Recently,Fused-MBConv is propo"}]}]}
>```
>%%
>*%%PREFIX%%se convolu-tions (Sifre, 2014).%%HIGHLIGHT%% ==Depthwise convolutions have fewerparameters and FLOPs than regular convolutions, but theyoften cannot fully utilize modern accelerators== %%POSTFIX%%. Recently,Fused-MBConv is propo*
>%%LINK%%[[#^kga5emiub4l|show annotation]]
>%%COMMENT%%
>why depthwise convolutions 
>+ fewer paramters
>- cannot be utilized fully on accelerators
>%%TAGS%%
>
^kga5emiub4l


>%%
>```annotation-json
>{"created":"2025-02-22T01:45:44.088Z","text":"replacing these depthwise blocks early on yields improved speed, but for all of them does not.\n\nThe count and placement of MBConv and Fused-MBConv layers can ideally be automatically ","updated":"2025-02-22T01:45:44.088Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":12532,"end":13007},{"type":"TextQuoteSelector","exact":"When applied in early stage 1-3, Fused-MBConv can improve training speed with a small overheadon parameters and FLOPs, but if we replace all blocks withFused-MBConv (stage 1-7), then it significantly increasesparameters and FLOPs while also slowing down the train-ing. Finding the right combination of these two buildingblocks, MBConv and Fused-MBConv, is non-trivial, whichmotivates us to leverage neural architecture search to auto-matically search for the best combination","prefix":"B4 with Fused-MBConv (Table 3). ","suffix":".depthwiseconv3x3SEMBConvconv1x1"}]}]}
>```
>%%
>*%%PREFIX%%B4 with Fused-MBConv (Table 3).%%HIGHLIGHT%% ==When applied in early stage 1-3, Fused-MBConv can improve training speed with a small overheadon parameters and FLOPs, but if we replace all blocks withFused-MBConv (stage 1-7), then it significantly increasesparameters and FLOPs while also slowing down the train-ing. Finding the right combination of these two buildingblocks, MBConv and Fused-MBConv, is non-trivial, whichmotivates us to leverage neural architecture search to auto-matically search for the best combination== %%POSTFIX%%.depthwiseconv3x3SEMBConvconv1x1*
>%%LINK%%[[#^zpj9br6imz|show annotation]]
>%%COMMENT%%
>replacing these depthwise blocks early on yields improved speed, but for all of them does not.
>
>The count and placement of MBConv and Fused-MBConv layers can ideally be automatically 
>%%TAGS%%
>
^zpj9br6imz


>%%
>```annotation-json
>{"created":"2025-02-22T01:47:16.707Z","text":"MBConv and Fused-MBConv","updated":"2025-02-22T01:47:16.707Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":12232,"end":12387},{"type":"TextQuoteSelector","exact":"It replaces the depthwise conv3x3 and expansion conv1x1in MBConv (Sandler et al., 2018; Tan & Le, 2019a) with asingle regular conv3x3, as shown in Figure 2","prefix":"e mobile or server accelerators.","suffix":". To system-atically compares th"}]}]}
>```
>%%
>*%%PREFIX%%e mobile or server accelerators.%%HIGHLIGHT%% ==It replaces the depthwise conv3x3 and expansion conv1x1in MBConv (Sandler et al., 2018; Tan & Le, 2019a) with asingle regular conv3x3, as shown in Figure 2== %%POSTFIX%%. To system-atically compares th*
>%%LINK%%[[#^hygva6z0ols|show annotation]]
>%%COMMENT%%
>MBConv and Fused-MBConv
>%%TAGS%%
>
^hygva6z0ols


>%%
>```annotation-json
>{"created":"2025-02-22T01:48:19.469Z","text":"this work adds in scaling the depth (# of layers) of the model  over training as well as changes image size progressively","updated":"2025-02-22T01:48:19.469Z","document":{"title":"EfficientNetV2: Smaller Models and Faster Training","link":[{"href":"urn:x-pdf:b7c05eaab5ac3c813cad1d438a300219"},{"href":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf"}],"documentFingerprint":"b7c05eaab5ac3c813cad1d438a300219"},"uri":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","target":[{"source":"vault:/devnotes/ML/OD%20papers/prejohned/efficientnetv2.pdf","selector":[{"type":"TextPositionSelector","start":13923,"end":14238},{"type":"TextQuoteSelector","exact":"we will use a non-uniform scaling strategy to gradually addmore layers to later stages. In addition, EfficientNets ag-gressively scale up image size, leading to large memoryconsumption and slow training. To address this issue, weslightly modify the scaling rule and restrict the maximumimage size to a smaller value","prefix":"meter efficiency. In this paper,","suffix":".3.3. Training-Aware NAS and Sca"}]}]}
>```
>%%
>*%%PREFIX%%meter efficiency. In this paper,%%HIGHLIGHT%% ==we will use a non-uniform scaling strategy to gradually addmore layers to later stages. In addition, EfficientNets ag-gressively scale up image size, leading to large memoryconsumption and slow training. To address this issue, weslightly modify the scaling rule and restrict the maximumimage size to a smaller value== %%POSTFIX%%.3.3. Training-Aware NAS and Sca*
>%%LINK%%[[#^q8kcqlzjcbs|show annotation]]
>%%COMMENT%%
>this work adds in scaling the depth (# of layers) of the model  over training as well as changes image size progressively
>%%TAGS%%
>
^q8kcqlzjcbs
