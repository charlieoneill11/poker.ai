# poker.ai
End-to-end poker augmented computer vision system. The process mirrors the structure of the repo:
1. Use the Raspberry Pi and OpenCV to pass images of both the table cards and hand cards to the model. The code for this is located in [pi](https://github.com/charlieoneill11/poker.ai/tree/main/pi).
2. After training an object detection model (YOLO3), we have the capacity to identify bounding boxes for cards in the image, and then to classify each individual card. The code for this is located in [vision](https://github.com/charlieoneill11/poker.ai/tree/main/vision).
3. The cards on the table and the player's hand is then passed to [poker](https://github.com/charlieoneill11/poker.ai/tree/main/poker), which determines the probabilities of winning based on the current hand. 
4. Based on the probabilities, [text](https://github.com/charlieoneill11/poker.ai/tree/main/text) then sends a text message to the player's smartwatch telling them whether they should fold, call or raise.
