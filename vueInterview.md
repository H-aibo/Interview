1. vue的生命周期
  > vue的生命周期主要分四个阶段：创建过程(beforeCreate, created)，挂载过程(beforeMount, mounted)，更新过程(beforeUpdate, updated)，销毁过程(beforeDestroy，destroyed)；
  > 在服务端渲染期间被调用的只有beforeCreate、created
  - beforeCreate（创建前）：当前生命周期el与data尚未初始化还不能访问data、computed、watch、methods上的方法和数据
  - created（创建后）：当前生命周期data初始化完成，可以访问到data、computed、watch、methods上的方法和数据，el初始化还没完成所以还不能访问
  - beforeMount（挂载前）：当前生命周期在挂载开始之前被调用`挂载元素，获取到DOM节点`
  - mounted（挂载后）：当前生命周期el已经挂载到文档里`可以操作DOM节点`
  - beforeUpdate（更新前-多次）：当前生命周期在数据更新的时候就会执行`更新的数据和模板还没结合，可以在当前生命周期做一个数据的最后修改`
  - updated（更新后-多次）：当前生命周期更新的数据与模板结合完毕`可以做一个确认停止事件的确认框`
  - activated：被keep-alive缓存的组件激活时调用
  - deactivated：被keep-alive缓存的组件停用时调用
  - beforeDestroy（销毁前-常用）：实例销毁前调用`当前生命周期做一些移除操作。例如：监听的移除，定时器的移除，事件的绑定`
  - destroyed（销毁后）：当前生命周期数据与视图之间的关系将会断开
  
