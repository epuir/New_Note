- # ![重要](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAB2EAAAdhAZXDuLYAAAFCSURBVDhPnZNRTsMwDIbtthJ7GxXjmXECxibedwN2A8oN9hoJCU1C9BrrDcYN4BkV6A32DlPHG0htgx2yqEm7afBJUX4ntePELuziIx5GPLTZiqfnbUQgcap1K6jnBvndxaDyq1fWXumdhzfPb2rDYWsG5GxOrmsXfI9HY60tUMICEbqspYRPiTBRGw64ikdzmq9+zT+TqDf4Z5DkSKSRegMWvMB6H+hKmfdVqHexqrBPJuzsfxfjcJat2W6UcXU/XADipTYtXGemWUZEs9kA5bruzFgZ5Ldnh+VBsNyUrw0PitNQZEtt2hmUHX/iOnMPaKmoZGA1lRWAmsc0iwT5xKf5WAwoyoNepnX6P2qYK3D6VSfI1Ykopz3xwhUxcMfSx3MaJxT8erNvMuD0aUrolfuuM3Ms0seeSPskZwio2x/gBxXHd1j10YF/AAAAAElFTkSuQmCC) **tranform****操作**

##      **//获取位置**

​    `Debug.Log(transform.position);`

​    `Debug.Log(transform.localPosition);`

##      **//旋转**

​    `Debug.Log(transform.rotation);`

​    `Debug.Log(transform.localRotation);`

​    `Debug.Log(transform.eulerAngles);`

​    `Debug.Log(transform.localEulerAngles);`

##     **//缩放**

​    `Debug.Log(transform.localScale);`

##     **//向量**

​    `Debug.Log(transform.forward);`

​    `Debug.Log(transform.right);` 

​    `Debug.Log(transform.up);`

##     **//时时刻刻看向000**

​    `//transform.LookAt(Vector3.zero);`

##      **//旋转**

​    `//transform.Rotate(Vector3.up,1);`

##      **//绕某个物体旋转**

​    `//transform.RotateAround(Vector3.zero, Vector3.up, 5);`

##      **//移动每一帧0.1**

​    `//transform.Translate(Vector3.forward * 0.1f);`

##      **//父子关系**

##     **//子物体个数**

​    `Debug.Log(transform.childCount);`

##     **//获取父物体**

​    //transform.parent.gameObject

##      **//解除父子关系**

​    `transform.DetachChildren();`

##      **//****获取子物体**

​    `Transform trans = transform.Find("Child");`

​    `Transform trans = transform.GetChild(0);`

##     **//判断是不是另外一个物体子物体**

​    `bool res = trans.IsChildOf(transform);`

​    `Debug.Log(res);`

##     **//设置为父物体**

​    `trans.SetParent(transform);`