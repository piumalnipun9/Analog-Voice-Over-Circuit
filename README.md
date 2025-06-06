# **Analog Voice-Over Circuit with Channel Prioritization**

This project demonstrates a fully analog implementation of a **Voice-Over Circuit** that effectively handles **two audio channels**, with automatic prioritization of the active channel.

## **Key Features**

- **Channel Prioritization**  
  Automatically prioritizes one channel when an input is detected, ensuring the most important channel is always heard.

- **Independent Volume Control**  
  Allows separate volume adjustments for both channels to tailor the audio output to specific needs.

- **Detection Threshold**  
  Adjustable detection threshold to ensure precise activation based on audio intensity.

- **Purely Analog Design**  
  Developed entirely using basic analog components and ICs, without digital processors, ensuring high-fidelity signal processing.

## **Functionality**

### 🔰 **Band-Pass Filter**  
The journey begins with a **band-pass filter**, which effectively improves the audio signal by reducing unwanted feedback and filtering out high-frequency noise. This step ensures that only the desired frequency range passes through for further processing.

### 🔰 **Pre-Amplifier**  
The filtered signal is then fed to a **pre-amplifier**, which boosts the signal to a level suitable for detection by the subsequent **peak detector circuit**. This ensures that the signal strength is sufficient for accurate analysis.

### 🔰 **Peak Detector Circuit**  
The **peak detector** captures the maximum amplitude of the audio signal, providing a stable DC output that is proportional to the peak amplitude. This step ensures that the highest level of the signal is preserved for accurate evaluation.

### 🔰 **Comparator Circuit**  
Next, the output from the peak detector is evaluated by a **comparator**. The comparator compares the peak value against a **predetermined threshold** and produces a high output when the signal surpasses this threshold. This decision determines whether audio from one channel or another should be activated.

### 🔰 **Control Signal for Switching**  
The **comparator's output** serves as a control signal to efficiently switch between the microphone input and the audio input. The priority channel is selected based on the detection of audio input.

### 🔰 **Main Amplifier**  
The final step involves the **main amplifier**, which amplifies the selected audio signal to a level that can be clearly heard through the **speaker**. The amplification ensures the output is loud and clear.

---

## **What We Learn From This Project**

- **Analog Signal Processing**  
  We gain hands-on experience in designing and implementing various analog circuits such as filters, amplifiers, and detectors. This emphasizes the importance of analog signal conditioning in real-world applications.

- **Audio Channel Management**  
  We learn how to handle multiple audio channels, manage input priorities, and ensure a seamless transition between them based on real-time detection, a valuable skill in audio systems and communication devices.

- **Threshold Detection and Signal Control**  
  This project teaches us how to use **thresholds** for activating or switching channels based on audio signals, a technique used in various applications like voice-activated systems and automatic switching systems.

- **Practical Circuit Integration**  
  Integrating multiple analog components—filters, amplifiers, detectors, comparators—into a cohesive working system gives us insight into how different analog devices can work together to form a complex functional unit.

---

## **Visuals of the Project**



- **PCB Design:**  
  ![PCB Design](https://github.com/ThilinaNirmalBandara/Analog-Voice-Over-Device/blob/e1cf411c256b8b1af5544d0714d4765a2282a1cc/pcb.jpeg)
  
- **Product Images:**  
  ![Product Images](https://github.com/ThilinaNirmalBandara/Analog-Voice-Over-Device/blob/318dd59bc88416f0e50e63e3511de1af58523332/enc.jpeg)
  ![Product Images](https://github.com/ThilinaNirmalBandara/Analog-Voice-Over-Device/blob/30659c403599d065a72fd0dfa7f771a78b525c63/enc1.jpeg)
  ![Product Images](https://github.com/ThilinaNirmalBandara/Analog-Voice-Over-Device/blob/1a46847465cda73cc1463e89158aae374ca129cb/enc3.jpg)
  
- **Signal Flow Diagram:**  
  ![Signal Flow Diagram](https://github.com/ThilinaNirmalBandara/Analog-Voice-Over-Device/blob/679a9b1e865f342f0b4994b55c33be4710e8329a/SignalFlow.jpg)

---
![Video Demo](https://github.com/ThilinaNirmalBandara/Analog-Voice-Over-Device/blob/0a98f55dccdce1c27985faf1868a9e6a9666198b/test%20video.mp4)
## **Components Used:**
- Band-pass filter
- Pre-amplifier IC
- Peak detector circuit
- Comparator IC
- Main amplifier IC
- Various passive components (resistors, capacitors)
## **Specific ICs Used:**
- LM386 for amplifier circuits
- NE5532 for other circuits
---

By completing this project, we develop a deeper understanding of analog systems, gain skills in circuit design and troubleshooting, and enhance our ability to create complex systems using only analog components.

Feel free to fork this repository and contribute to further improvements or modifications!

