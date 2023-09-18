#                               *unity笔记*

##                   **unity**     场景的操作

###     **//场景跳转** 

​    `SceneManager.LoadScene(0,LoadSceneMode.Additive);`

###     **//获取当前场景**

​    `Scene sene = SceneManager.GetActiveScene();`

###     **//场景名称**

​    `Debug.Log(sene.name);`

###     **//场景是否加载**

​    `Debug.Log(sene.isLoaded);`

###     **//场景路径**

​    `Debug.Log(sene.path);`

###     **//场景索引**

​    `Debug.Log(sene.buildIndex);`

​    `GameObject[] gos = sene.GetRootGameObjects();`

​    `Debug.Log(gos.Length);`

​    `GameObject a;`

​    `a = gos[0];`

​    `Debug.Log(a.name);`

###     **//场景管理**

​    `Debug.Log(SceneManager.sceneCount);`

###     **//创建新场景**

​    `Scene newScene = SceneManager.CreateScene("newScene");`

​    `Debug.Log(SceneManager.sceneCount);//激活场景个数`

###     **//卸载场景**

  `SceneManager.UnloadSceneAsync(newScene);`