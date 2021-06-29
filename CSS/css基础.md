### 1. 清除浮动（双伪类）
    > 可以清除浮动，可以解决外边距塌陷
  ```css
  .clearfix::before,
  .clearfix::after {
    conent: '',
    display: table;
  }
  .clearfix::after {
    clear: both;
  }
  ```
