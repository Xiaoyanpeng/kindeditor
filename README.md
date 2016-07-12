# kindeditor
富文本使用
```
<link rel="stylesheet" href="kindeditor/themes/default/default.css" />

<script charset="utf-8" src="kindeditor/kindeditor-min.js"></script>
<script charset="utf-8" src="kindeditor/lang/zh_CN.js"></script>

<script>
          var editor;
          KindEditor.ready(function(K) {
            editor = K.create('textarea[name="desc"]', {
              afterBlur:function(){this.sync()},   //使用ajax时才需要，非button
              resizeType : 1,
              allowPreviewEmoticons : false,
              allowImageUpload : false,
              items : [
                'fontname', 'fontsize', '|', 'forecolor', 'hilitecolor', 'bold', 'italic', 'underline',
                'removeformat', '|', 'justifyleft', 'justifycenter', 'justifyright', 'insertorderedlist',
                'insertunorderedlist', '|', 'emoticons', 'image', 'link']   
            })
          })
    </script>
    ```
