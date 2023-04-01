## Ablation Studies.

In this part, we perform an relative AU~(RAU) ablation experiment to verify the effectiveness of the introduced relative AU constraint. The comparison results are shown below.
### ---------------Driving ME---------------------------
<div style="align: center">
<img src="gifs/Driving_ME.gif"/>
</div>
### ---------------Template_Female_Asia---------------------------

1.Only TPS

<div style="align: center">
<img src="gifs/1-only TPS.gif"/>
</div>

2.TPS+RAU

<div style="align: center">
<img src="gifs/1-TPS+RAU.gif"/>
</div>



### ---------------Template_Female_Europe---------------------------
1.Only TPS

<div style="align: center">
<img src="gifs/2-only TPS"/>
</div>

2.TPS+RAU

<div style="align: center">
<img src="gifs/2-TPS+RAU.gif"/>
</div>

### Conclusion
Comparing the generated results of "1-only TPS.gif" and "1-TPS+RAU.gif", it can be observed that when RAU is not introduced, a slight and unreasonable upward stretch motion appears at the "left corner of the mouth" on the generated micro-expression in the target face compared to the source micro-expression. However, after introducing RAU, this irrelevant motion disappears, which intuitively proves that the introduced RAU can indeed suppress the irrelevant motion in the facial area caused by motion estimation.
	
Comparing the generated results of "2-only TPS.gif" and "2-TPS+RAU.gif", it can be seen that when RAU is not introduced, the generated model overlooks the slight motion of "left eyelid contraction" in the source micro-expression. However, with RAU, the model can handle this local detail very well, which reflects that the introduction of relative AUs can enhance the generation model's attention to the fine-grained motion in the facial local area.

This indicates that AU constraint to some extent helps our model understand more about semantics of the expression and helps to generate fine-grained micro-expressions.

