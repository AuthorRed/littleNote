总体目标
  解决人们要记录的笔记越来越多,用树形结构来记录笔记,方便后续的查找和分类
现状
  第一次提交只是实现了记笔记的锥形,笔记保存在本地储存localStorage中
下一步目标
  修复节点修改不稳定的bug
    这个问题是由于当对一个节点修改还没有结束时,再去增删改其他节点时就可能会引起父节点不稳定而导致的
      可以尝试通过所机制来解决这个问题,修改前要先获取锁,没有锁不让修改;
        ztree有提供beforeRename & onRename这样的api来控制
  实现搜索框查找节点功能
  实现拖拽拼接功能
  实现前进后退功能
  实现按照录入时的索引来排序,而非现在默认的排序方法
  添加导入导出笔记的功能
    现在的笔记是以JSON形式储存在浏览器上,通过添加textarea来实现导入导出
  添加删除所有数据的弹出框确认
