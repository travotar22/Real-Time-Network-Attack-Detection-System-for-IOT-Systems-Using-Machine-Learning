# Real-Time-Network-Attack-Detection-System-for-IOT-Systems-Using-Machine-Learning
This project captures real-time network traffic using Scapy, extracts essential packet features, and preprocesses them for a KNN classifier. The pre-trained model then determines if a packet indicates malicious activity. It aids network administrators in monitoring for suspicious activities in real-time.

Packet Analysis for Malicious Traffic Detection

This project is a real-time network traffic analyzer that captures packets from a specified network interface using Scapy. Each captured packet is processed to extract essential features such as IP addresses, transport layer details, TCP/UDP flags, and packet size. These features are then pre-processed, and redundant or non-numeric data like IP addresses are removed. Additionally, categorical data like the protocol type (TCP, UDP, or OTHER) are one-hot encoded for model compatibility.

Once processed, these features are passed through a pre-trained K-Nearest Neighbors (KNN) classifier to predict whether the packet indicates malicious or benign activity. The result for each packet is then printed in real-time, allowing network administrators or cybersecurity professionals to monitor their network for any suspicious activities.
