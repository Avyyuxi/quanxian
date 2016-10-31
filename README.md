## 查询test1 页面权限
![1](https://cloud.githubusercontent.com/assets/16081282/19842910/67b3463c-9f58-11e6-99b5-abd38f633dc4.PNG)
## 查询结果
![1](https://cloud.githubusercontent.com/assets/16081282/19842966/015b95fa-9f59-11e6-890f-180692c04151.png)
#### 伪代码
1、根据用户名称查询UserID

2、根据用户ID查对应角色RoleIDs

3、权限表页面表并查找

   角色类型为CF_Role AND 角色编号在角色RoleIDs中

  OR

  角色类型为CF_User AND 人员编号为UserID

4、判断权限集合是否有查看权限输出对应页面

## 查询test1 操作权限
![2](https://cloud.githubusercontent.com/assets/16081282/19843077/0cffc40c-9f5a-11e6-8cfc-14e8dd20a385.PNG)
## 查询结果
![2](https://cloud.githubusercontent.com/assets/16081282/19843106/24fc8bf8-9f5a-11e6-89fd-e81cce685b6c.png)
#### 伪代码
1、根据名称查找人员编号UserID

2、根据人员编号UserID查找改人员所对应的角色RoleIDs

3、权限表按钮表页面表并查找

   角色类型为CF_Role AND 角色编号在角色RoleIDs中
 OR
          角色类型为CF_User AND 人员编号为UserID

4、  查询权限集合中菜单名为“订单”的数据
