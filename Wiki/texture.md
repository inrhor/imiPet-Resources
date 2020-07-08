#有关纹理与模型的显示
***
#####前言
> **[warning]** 请注意
>
> 这里仅讲纹理与部件显示的有关内容，若想学习模型制作，请另寻教程
> 
> 所有模型的原版材质必须是钻石锄子


***
#####高清修复
高清修复就是OptiFine
``` yaml
pets:
  # 关于模型与动态模型
  animation:
    # 空闲状态
    idle:
      # 物品名称
      itemName: "pet1"
```
我们来剖解纹理包看看
``` yaml
type=item
items=minecraft:diamond_hoe
nbt.display.Name=pet1
model=./head
```
可以看到，minecraft:diamond_hoe是钻石锄子的名称，pet1是物品名称
***
#####模型数据
如果不想要耐久值或高清修复，那么有模型数据值得选择  
请看：http://imipet.com/resources/17/
***
#####常见问题
> 纹理包版本过低？


提示旧版本是材质包内pack.mcmeta文件设置问题
``` yaml
{
  "pack": {
    "pack_format": 3
  }
}
```
请根据需要，修改数字  
1.12 pack_format=3  
1.13-1.14 pack_format=4  
1.15 pack_format=5  


> 如何将多个纹理包放入同一纹理包？


请看教程：http://www.imipet.com/threads/23/


> 纹理包是什么？客户端如何使用纹理包？


这么简单都不懂，纹理包也就是材质包，也就是资源包，我只是喜欢这么叫


纹理包放入客户端的位置：.minecraft\resourcepacks


然后在客户端按 ESC键，点击资源包，放入右侧完成后自动加载资源包