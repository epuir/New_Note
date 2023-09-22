#                                           unity简单射线系统

## 创造射线

##### 方式一

#### `Ray ray = new Ray(起点,方向);`

 `Ray ray = new Ray(Vector3.zero,Vector3.up);`

##### 方式二屏幕法创造

`Ray ray = Camera.main.ScreenPointToRay(Input.mousePosition);`

### 碰撞检测

`bool res = Physics.Raycast(ray, out RaycastHit hit;，float MaxDistance,int LayerMask);``//如果碰撞到返回值就有内容`

ray射线，hit 碰撞体信息，maxdistance最大距离，layermask图层如1<<10打开10图层（0为关闭，1为打开）

`LayerMask.GetMask("图层名称")`  = ~(0<<5&1<<9)

###### 如果碰撞为ture,否则为false

### 碰撞信息

RaycastHit 为碰撞信息结构体

point 碰撞位置  collider碰撞体的  rigidbody命中碰撞体的    transform射线原点到撞击点的距离

### 多检测

`RaycastHit[] hits = Physics.RaycastAll(ray, 100f, 1 << 10);`

结构体数组

### DeBug射线

##### 显示出具有方向和长度的向量

`DeBug.DrawRay(transform.position,transform.position+transform.forward*10,Color.yellow);`

##### 显示出线段

`DeBug.DrawLine(transform.position,hitInfo.poin,Color.yellow);`

### 线段检测

`LineCast(startpos,endPos,LayerMask.GetMask("LayerName"));`

`LineCast(startpos,endPos,out RaycastHit hit,LayerMask.GetMask("LayerName"));`

##### 返回bool类型

