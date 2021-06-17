1. vue的生命周期
  > vue的生命周期主要分四个阶段：创建过程(beforeCreate, created)，挂载过程(beforeMount, mounted)，更新过程(beforeUpdate, updated)，销毁过程(beforeDestroy，destroyed)
  - beforeCreate（创建前）：当前生命周期el与data尚未初始化还不能访问data、computed、watch、methods上的方法和数据
  - created（创建后）：当前生命周期data初始化完成，可以访问到data、computed、watch、methods上的方法和数据，el初始化还没完成所以还不能访问
  - beforeMount（挂在前）：当前生命周期在挂载开始之前被调用`挂载元素，获取到DOM节点`
  - mounted
  - beforeUpdate
  - updated
  - activated
  - deactivated
  - beforeDestroy
  - destroyed
  - errorCaptured
  
  
