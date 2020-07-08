#####API的一些用法
对实体添加模型  
1.使用已通过配置成功注册的宠物模型
```
Entity entity = ...;
String modelId = "模型ID"
ModelEntityManager modelEntityManager = new ModelEntityManager(entity, modelId);
ModelEntityManager.fastSpawnModel(modelEntityManager, modelId);
```

2.不使用注册的模型ID
```
Entity entity = ...;
String modelId = "模型ID"
ModelEntityManager modelEntityManager = new ModelEntityManager(entity, modelId);
modelEntityManager.setAnimationItemNameIdle("物品名称");
modelEntityManager.setAnimationItemNameWalk("物品名称");
modelEntityManager.setAnimationItemNameAttack("物品名称");
modelEntityManager.setAnimationCustomModelDataIdle(模型数据);
modelEntityManager.setAnimationCustomModelDataWalk(模型数据);
modelEntityManager.setAnimationCustomModelDataAttack(模型数据);
modelEntityManager.setModelLocationH(显示模型高度);
modelEntityManager.spawnModel();
```
