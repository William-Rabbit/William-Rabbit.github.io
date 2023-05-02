# HAL

## GPIO

### 概述


### 函数

#### 类型定义

##### GPIO初始化结构定义

```C
typedef struct
{
    uint32_t Pin;           /*指定需要配置的GPIO引脚,该参数可以是GPIO_pins的值之一*/
    uint32_t Mode;          /*指定所选引脚的操作模式,该参数可以是GPIO_mode的值之一*/
    uint32_t Pull;          /*指定所选引脚的上拉/下拉方式,该参数可以是GPIO_pull的值之一*/
    uint32_t Speed;         /*指定所选引脚的速度,该参数可以是GPIO_spend的值之一*/
    uint32_t Alternate;     /*将外设连接至所选的引脚,该参数可以是GPIOx_Alternate_function_selection的值之一*/
}GPIO_InitTypeDef;
```

##### GPIO位置位和复位枚举

```C
typedef enum
{
    GPIO_PIN_RESET = 0,
    GPIO_PIN_SET
}GPIO_PinState;
```

#### 常量定义

##### GPIO_pins定义

|  状态定义  |    释义     |  状态定义  |    释义     |
| :--------: | :---------: | :--------: | :---------: |
| GPIO_PIN_0 | 引脚0被选择 | GPIO_PIN_8 | 引脚8被选择 |
| GPIO_PIN_1 | 引脚1被选择 | GPIO_PIN_9 | 引脚9被选择 |
| GPIO_PIN_2 | 引脚2被选择 | GPIO_PIN_10 | 引脚10被选择 |
| GPIO_PIN_3 | 引脚3被选择 | GPIO_PIN_11 | 引脚11被选择 |
| GPIO_PIN_4 | 引脚4被选择 | GPIO_PIN_12 | 引脚12被选择 |
| GPIO_PIN_5 | 引脚5被选择 | GPIO_PIN_13 | 引脚13被选择 |
| GPIO_PIN_6 | 引脚6被选择 | GPIO_PIN_14 | 引脚14被选择 |
| GPIO_PIN_7 | 引脚7被选择 | GPIO_PIN_15 | 引脚15被选择 |
| GPIO_PIN_ALL | 所有引脚被选择 |            |             |

##### GPIO_mode定义

|      状态定义       |       释义       |           状态定义           |               释义                |
| :-----------------: | :--------------: | :--------------------------: | :-------------------------------: |
|   GPIO_MODE_INPUT   |   浮空输入模式   |     GPIO_MODE_IT_RISING      |   上升沿触发检测的外部中断模式    |
| GPIO_MODE_OUTPUT_PP |   推挽输出模式   |     GPIO_MODE_IT_FALLING     |   下降沿触发检测的外部中断模式    |
| GPIO_MODE_OUTPUT_OD |   开漏输出模式   | GPIO_MODE_IT_RISING_FALLING  | 上升/下降沿触发检测的外部中断模式 |
|   GPIO_MODE_AF_PP   | 复用功能推挽输出 |     GPIO_MODE_EVT_RISING     |   上升沿触发检测的外部事件模式    |
|   GPIO_MODE_AF_OD   | 复用功能开漏输出 |    GPIO_MODE_EVT_FALLING     |   下降沿触发检测的外部事件模式    |
|  GPIO_MODE_ANALOG   |     模拟模式     | GPIO_MODE_EVT_RISING_FALLING | 上升/下降沿触发检测的外部事件模式 |

##### GPIO_speed定义

|       状态定义       | 释义 |         状态定义          |  释义  |
| :------------------: | :--: | :-----------------------: | :----: |
| GPIO_SPEED_FREQ_LOW  | 低速 |  GPIO_SPEED_FREQ_MEDIUM   |  中速  |
| GPIO_SPEED_FREQ_HIGH | 高速 | GPIO_SPEED_FREQ_VERY_HIGH | 超高速 |

注: 不同频率实质为信号上升沿与下降沿所需要的时间长短不同,频率越高,所需时间越短,但因此功耗就会增大

##### GPIO_pull定义

|   状态定义    |     释义     |  状态定义   |     释义     |
| :-----------: | :----------: | :---------: | :----------: |
|  GPIO_NOPULL  | 无上下拉电阻 | GPIO_PULLUP | 激活上拉电阻 |
| GPIO_PULLDOWN | 激活下拉电阻 |             |              |

#### 函数定义

