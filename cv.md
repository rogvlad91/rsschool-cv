# Vladislav Rogov
**Mobile:**+79140204737 **E-mail:**rogvlad91@gmail.com
## Profile
A motivated, adaptable and responsible Mobile Systems graduate pursuing a position in IT. I have over half a year experience in engineering. My current job requires solving different programming problems with Matlab.
## Skills
* MATLAB 
* Basic front-end skills: HTMl, CSS
* Basic knowledge of Git 
* Altium Designer 
* Basic C++ skills
## Code example
```function [Q, R] = QR_house(A)
%   QR decomposition using Householder reflections
%   Input:  A - Hermitian matrix
%   Output: Q - unitary matrix
%           R - upper-triangle matrix
 
[r, ~] = size(A); 
Q = eye(r);
I = eye(r);
k =  1;
    for i = 1 : r - 1    
        v = zeros(1,r);
        v(k) = A(k,k) + (A(k,k))./abs((A(k,k))) * sum(A(:,k), k); %Householder vector
        for j = k + 1 : r
            v(j) = A(j,k);
        end
        H = I - 2 * ( conj(v' * v) / (v * v')); %Householder matrix
        Q = Q * H;
        A = H * A;
        k = k + 1;
    end
 
R = A;
end
```
## Experience 
* 2021-present moment Engineer on NII Vector. Developing various scripts and algorithms for radio engineering needs in Matlab
## Education 
Bachelor Mobile Communication Systems 
Saint-Petesburg Electrotechnical University 
2017-2021
## Languages 
* English C1
* German B1