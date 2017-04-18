# simple-pubsub

  > simple pubsub

## API
  
  * PubSub.subscribe(subName, function) 订阅subName, @subName(必传): 订阅名称；@function(必传): 订阅的回调函数，返回此订阅的唯一token，否则return false
  
  * PubSub.publish(subName, data) 发布订阅信息, @subName(必传): 订阅名称；@data: 传递的信息数据, 返回Boolean
  
  * PubSub.unSubscribe(subName, token)/PubSub.cancelSubscribe(subName, token)  取消某单个订阅信息, @subName(必传): 订阅名称；@token: 订阅的唯一token(token为空，则取消名称为subName的所有订阅), 返回Boolean
  
  * PubSub.clearSubscribe(subName) 取消名称为subName的所有订阅, @subName: 订阅名称；返回Boolean
  
  * PubSub.clearAllSubscribe() 清空所有的订阅, 返回Boolean
