# JSX

## type 类型别名
type Props = {};

type State = {};

变量？和？类型的区别

```javascript
type Props = {
    // (MODAL_TYPE_RN_MODAL类型不起作用，永远是垂直方向动画)
    // orientation属性 默认定义content内容flexDirection
    orientation?: CONTENT_ORIENTATION, // slide动画方向 ORIENTATION_LANDSCAPE:水平动画 ,ORIENTATION_PORTRAIT:垂直动画
    modalType?: MODAL_VIEW_TYPE,
    animationType?: MODAL_ANIMATION_TYPE,
    contentCenter?: Boolean, // Modal内容是否居中显示 默认不居中
    useNativeDriver?: Boolean,
    canceledOnTouchOutside?: Boolean, // 点击内容之外是否隐藏Modal 默认隐藏
    overlayStyle?: Object | Number, // 自定义蒙层 style
    onRequestClose?: () => void, // android 物理返回键点击回调
    onTouchOutside?: () => void, // 内容之外点击回调
};
```

```javascript
autoDismissTimer: ?Timer = null; // modal显示5s后自动隐藏
```

## 生命周期函数

需要注意构造函数添加 this.destroyed = true; // 当前页面是否销毁