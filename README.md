# Perception-Pyramid-Network
Understanding Scene Evolution from LiDAR Perception in Autonomous Racing
# Abstract:
Autonomous driving when applied for high-speed racing aside for urban environments presents unique challenges due to dynamic nature of racing circuits and the need for optimal future plannings at high speeds. While simulator-based approaches, CARLA, Air Sim, TORCS provide clean environment data to models but transfer learning to real-world is a hard problem. In this paper, we propose leveraging LiDAR data obtained from the real-world to train a deep learning network to understand and predict the future states of the perceived scenes. The proposed network, named Perception Pyramid Network (PPN), takes a sequence of past environment scans plus the current scan, and learns how the environment evolves over a sequence of future timesteps. Due to limitation of processing raw point clouds in directly capturing spatial relationships between points, the 3D point clouds obtained from LiDAR sweeps are converted into 2D Bird’s Eye View map, which encodes information in each grid cell. PPN is a type of encoder-decoder network which extracts these features, across both space and time, in a hierarchical fashion resembling the pyramid shape. The network is trained with a combination of loss functions and exhibits a real-time inference frequency of ~16 Hz on a NVIDIA Tesla P100 GPU. Implementation is available at: https://github.com/suwesh/Perception-Pyramid-Network. 

![encoderdecoder-highlevel](https://github.com/suwesh/Perception-Pyramid-Network/assets/83471963/ad95179f-80e5-4cf6-8ce9-58665a08dc53)
