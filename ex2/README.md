Logistic Regression

plot(X,Y,'k+') 打印+号
plot(X,Y,'ko') 打印o

Cost function and gradient
	代价函数与梯度与线性回归类似

fminunc:
	options = optimset('GradObj','on','MaxIter',400);
	[theta,J,exit_flag] = fminunc(@(t)(costFunctionReg(t,X,y,lambda)),initial_theta,options);
