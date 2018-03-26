# wepy-popup




```sh

<popup
    :visibility.sync="{{visibility}}"
    type="top"
    className="popup-class-name"  
    @onShow.user="onPopupShow" @onHide.user="onPopupHide">

    <view slot="content">弹窗内容</view>

</popup>


data = {
    visibility:'visible',
}
....
components = {
    popup: popup,
}

```
## 参数说明
```js
    {
        visibility, //必填，控制浮层显隐，可选值 `visible`,`hidden`
        type, //浮层方向，默认'bottom'，可选值 `top`,`bottom`,`center`
        className, // 添加css类名
    }

  methods = {
      onPopupShow(){

      },
      onPopupHide(){

      }
  }

  //弹窗内容 通过slot='content' 传入
```

## 示例效果图
![效果图](http://f2er.meitu.com/zhy/npm_images/wepy-popup-eg.png)
