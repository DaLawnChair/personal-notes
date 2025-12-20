Encoder-Decoder architecture:

Encoder:
* takes input tokens 
* processes through mutliple attention layers
* outputs contextual embeedings representing each token

Decoder:
* takes encoder output and previous decoder outputs
* generates tokens step by step
* uses additional attention mechanism to focus on relevant encoder outputs


Self-attention:
* Input vectors Q (Query), K (Key), and V (value)
* **Q (Query)**: The current token trying to understand its relation to others.
- **K (Key)**: The tokens being compared against.
- **V (Value)**: The actual information being retrieved.
- **\sqrt{d_k}​​**: A scaling factor to keep gradients stable.

Multihead attention:
$MultiHead(Q,K,V)=Concat(head_1​,…,head_h​)W^O$
Each head is for $W^Q,W^K,W^V$ to focus on semantic aspects

Positional Encoding
transfomers process in parrallel, so they do not understand word order. Positional encodings are added as input embeddings,

PE(pos,2i)​=sin(pos/100002i/dmodel​) 
PE(pos,2i+1)=cos⁡(pos/100002i/dmodel)

Feed Forward Network (FFN):
applied independently to each token
$FFN(x)=max(0,xW_1​+b_1​)W_2​+b2_​$

Layer Normalization & Residual Connections
uses skip connections
LayerNorm(x+Attention(x))
