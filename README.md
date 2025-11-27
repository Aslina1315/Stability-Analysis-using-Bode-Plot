# Stability-Analysis-using-Bode-Plot
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=1/(S(1+0.5S)(1+0.1S)) using bode plot and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![WhatsApp Image 2025-11-27 at 22 34 45_7222e77b](https://github.com/user-attachments/assets/53c6079a-f43d-4103-b049-5c4b1deb090f)
![WhatsApp Image 2025-11-27 at 22 34 54_578df6bc](https://github.com/user-attachments/assets/10741906-ebd8-4641-8b05-0e4081b6fc6b)
![WhatsApp Image 2025-11-27 at 22 36 13_37657e15](https://github.com/user-attachments/assets/99f42e43-2517-4873-bc11-e66c2189fab4)
![WhatsApp Image 2025-11-27 at 22 35 07_322743ab](https://github.com/user-attachments/assets/a2b844f4-e6f1-4e89-99f3-f321bbf458e3)





## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Determine the gain crossover frequency, phase cross over frequency, gain margin and phase margin.
	Also determine the stability.

## Program: 
num=1<br>
den=[0.05 0.6 1 0]<br>
sys=tf(num,den)<br>
bode(sys)<br>
grid on<br>
[Gm Pm Wpc Wgc]=margin(sys)<br>
if(Wpc>Wgc)<br>
disp('stable')<br>
elseif(Wpc == Wgc)<br>
disp('marginally stable')<br>
else<br>
disp('unstable')<br>
end<br>

## Output:

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/6f7b6990-51d6-4681-beb6-009442d2b38d" />

## Result:
Thus the bode plot for the given transfer function was drawn and verified using MATLAB. <br>
Gain margin = 12.0
Phase Margin = 60.42
Gain crossover frequency = 0.907
Phase crossover frequency = 4.4721
The system is stable 
