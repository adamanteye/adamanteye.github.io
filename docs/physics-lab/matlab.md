## 一般直线回归拟合

```m
y_mes = []; % 此处填充数据，以;分割
x=[]; % 此处填充数据，以;分割

% 可选
% ln=@(x) log(x);
% x=arrayfun(ln,x);
% y_mes=arrayfun(ln,y_mes);


n=numel(x);

X = [ones(length(x),1) x];
b = X\y_mes;
y_cal=X*b;
v=n-2;
rss=sqrt(sum((y_mes-y_cal).^2));
sy=sqrt(rss/v);
sb1=sy/sqrt(sum((x-mean(x)).^2));
sb0=sy*sqrt(1/n+mean(x)^2/sum((x-mean(x)).^2));
tv=1.959+2.406/(v-1.064); % p=0.95
ub0a=tv*sb0;
ub1a=tv*sb1;

% 绘图
scatter(x,y_mes,'filled')
hold on
% xlim();
% ylim();
set(gca,'FontName','Times New Roman');
plot(x,y_cal)
xlabel('') % 此处填充x轴标签
ylabel('') % 此处填充y轴标签
title('') % 此处填充标题
grid on

print('',"-dpng"); $ 此处填充文件名
```

## LSM 拟合

```
y_mes = []; % 此处填充数据，以;分割
x=[]; % 此处填充数据，以;分割
n=numel(x);

b=x\y_mes;
y_cal=b*x;
v=n-1;
rss=sqrt(sum((y_mes-y_cal).^2));
sy=sqrt(rss/v);
sb=sy/sqrt(sum(x.^2));
tv=1.959+2.406/(v-1.064); % p=0.95
uba=tv*sb;

scatter(x,y_mes,'filled')
hold on
xlim([0,3.5]);
ylim([0,120]);
set(gca,'FontName','Times New Roman');
plot(x,y_cal)
xlabel('') % 此处填充x轴标签
ylabel('') % 此处填充y轴标签
title('') % 此处填充标题
grid on

print('',"-dpng"); $ 此处填充文件名
```

## 参考
