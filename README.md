

本项目Fork自 [AppianZ/multi-picker](https://github.com/AppianZ/multi-picker/tree/master/MultiPicker)

[原项目文档](./README_ORIGIN.md)

为`multi-picker`增加和修正了一些功能：

1. 采用*label*和*value*区分展示的值和真实的数据值

    ```js
    jsonData: [{
      value: 'test1',
      label: 'label1'
    }, {
      value: 'test2',
      label: 'label2'
    }],
    ```

2. 在初始化`new MultiPicker({})`时增加了default属性，type为`Array`，依次提供想要定位的值对应的id即可，如

    ```js
    // 福建省 - 厦门市 - 集美区 - aaa街道 - a1街道
    default: ['1203', '002', '2a', '2a-a', 'aaa-2']
    ```
3. `multi-picker-down-shadow`的`bottom`设置为0，使遮罩层看上去更为自然