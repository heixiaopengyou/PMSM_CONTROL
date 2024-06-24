# PMSM_CONTROL
Permanent Magnet Synchronous Motors (PMSMs) are brushless and have very high reliability and efficiency. 
They are widely used for high-performance drives such as industrial robots and machine tools because of their advantages as high efficiency, high power density, high torque/inertia ratio, and less maintenance.
Although these motors are highly demanded, the control of the PMSM is still a hot topic. Recent articles on PMSM plant linearization (using PID control) do not show convincing results.
Moreover the ideal controller in this case, the  Non Linear MPC (nlmpc) is almost impossible to implement on device.
Thus, this research is centered on using a neural network to approximate the efficiency of the nlmpc, which could be deployed on board.
After designing and training the network using information from the nlmpc, the model goes through the Net to Bytes workflow inorder to get the fasted inferred model, with minimum parameters.

The initial work (on PMSM control) which we use as reference is the #Field Oriented Control of a 3-Phase Permanent Magnet Synchronous Motot# proposed in the Data in Brief paper #https://www.data-in-brief.com/article/S2352-3409(23)00120-8/fulltext
