# my-vue-modal-loading-conponents
自己整理的vue项目中用到的弹窗和loading图标以及消息提示组件
## 使用方法

### 1.弹窗组件modal
将src/components/modal整个文件夹copy到你的项目中
在使用的页面中import改组件
使用该组件标签
```html
<i-modal :modal-show="isShow"
          width="30%"
          @handleClose="isShow=false"
          @onOk="isShow=false"
          @onCancel="isShow=false"
          @maskClosable="isShow=false">
       <div slot="body">
           <div>身体部分</div>
           <div>身体部分</div>
       </div>
</i-modal>
```
配置说明: width: modal宽度
handleClose:modal右上角点击叉号关闭的回调 
onOk:选择确定的回调 
onCancel:取消的回调
maskClosable:点击模态框关闭modal的回调
title: 弹窗的标题
slot="body": 插槽,在里面写入modal内容的html代码

### 2.加载中lodaing组件
将src/components/loading整个文件夹copy到你的项目中
在使用的页面中import改组件
使用该组件标签
```html
<loading
    load-name="bars"
    loading-title="加载中"
    :loading="loadingShow"> 
</loading>
```
配置说明:
load-name: 使用loading图标的样式,oval,spinning,ball,three,tail,puff,bars
loading-title: lodaing图标下面的文字说明
load-width: loading图标的大小

待续...
