18b20驱动使用注意事项：

1.IO口占用情况：接口定义：B6可以更换;

2.main函数中需要添加的头文件：

#include "18b20.h"

3.调用该函数必须调用DS18B20_RCC()进行时钟配置，然后调用返回值为u16的One_Change（）
函数即可得转换后的值，用该值乘以0.0625即可得到温度值。