![image](https://github.com/user-attachments/assets/05972796-b64b-4189-8c03-b482fae940d5)


This research investigates and improves the architecture of the lightweight convolutional neural network ShuffleNet-V2 with the aim of improving the performance in image classification on platforms with limited computational resources. The proposed structure, titled Overlapping ShuffleNet, uses the channel overlapping method in the channel division section to increase the information exchange between channels and provide a more accurate representation of features. In this architecture, the input is divided into three branches, including two branches with 38 channels and one branch with 40 overlapping channels, each of which is subjected to convolution operations, and then the outputs are merged as element-by-element sums and channel scrambling operations are applied to them. Experimental results from implementing the models on a dataset of dog and cat images consisting of 25,000 training images show that the accuracy of the proposed model reaches 87.6%, which is a significant improvement over the basic ShuffleNet-V2 model with an accuracy of 84.92%. It was also found that eliminating channel convolution or reducing convolutional layers causes a decrease in model accuracy. Finally, the findings show that combining channel overlap with channel convolution can provide an optimal balance between accuracy and processing speed and play a strategic role in designing effective neural networks for low-resource devices.

### Architecture      
![image](https://github.com/user-attachments/assets/a7720394-61ed-4172-af8e-17e3c6f93004)

![image](https://github.com/user-attachments/assets/c87cd377-e916-461f-ac6a-25ada1e3ea43)

--------------------------
### Sample DataSet    
![image](https://github.com/user-attachments/assets/2e34d387-1710-4ce7-8f61-d095511a170c)



----------------
### ShuffleNet v2 train & test                   
![image](https://github.com/user-attachments/assets/0bb00844-dd20-431d-aa2d-e8a70a128a00)




### ShuffleNet Overlapping (proposed method) train & test         
![image](https://github.com/user-attachments/assets/bbd001b0-4519-4953-9067-d190433f53d0)



### Results      
| Accuracy in Valid % | Has ChannelShuffle | Channel count overlap | Model                             |
| ------------------- | ------------------ | --------------------- | --------------------------------- |
| 84.92               | true               | -                     | ShuffleNet-V2                     |
| 81.82               | false              | -                     | ShuffleNet-V2                     |
| 77.89               | true               | 20                    | ShuffleNet overlap (2 layer Conv) |
| 83.6                | false              | 20                    | ShuffleNet overlap                |
| 84.48               | true               | 20                    | ShuffleNet overlap                |
| 82.34               | false              | 30                    | ShuffleNet overlap                |
| 85.0                | true               | 30                    | ShuffleNet overlap                |
| 82.54               | false              | 40                    | ShuffleNet overlap                |
| 87.6                | true               | 40                    | ShuffleNet overlap                |
| 82.0                | false              | 50                    | ShuffleNet overlap                |

### References

    Alex Krizhevsky, I. S. (2012). ImageNet Classification with Deep Convolutional Neural Networks. Advances in Neural Information Processing Systems (NIPS).
    Andrew G. Howard, M. Z. (2017). MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications. Computer Vision and Pattern Recognition (cs.CV).
    Chollet, F. (2017). Xception: Deep Learning with Depthwise Separable Convolutions. Computer Vision and Pattern Recognition (cs.CV).
    Christian Szegedy, W. L. (2014). Going Deeper with Convolutions. Computer Vision and Pattern Recognition (cs.CV).
    Forrest N. Iandola, S. H. (2016). SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size. Computer Vision and Pattern Recognition (cs.CV); Artificial Intelligence (cs.AI).
    Jie Hu, L. S. (2019). Squeeze-and-Excitation Networks. Computer Vision and Pattern Recognition (cs.CV).
    Kaiming He, X. Z. (2015). Deep Residual Learning for Image Recognition. Computer Vision and Pattern Recognition (cs.CV).
    Ningning Ma, X. Z.-T. (2018). ShuffleNet-V2: Practical Guidelines for Efficient CNN Architecture Design. Computer Vision and Pattern Recognition (cs.CV).
    Saining Xie, R. G. (2017). Aggregated Residual Transformations for Deep Neural Networks. Computer Vision and Pattern Recognition (cs.CV).
    Xiangyu Zhang, X. Z. (2017). ShuffleNet: An Extremely Efficient Convolutional Neural Network for Mobile Devices. Computer Vision and Pattern Recognition (cs.CV).


