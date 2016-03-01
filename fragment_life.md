### 官网文档链接 <http://developer.android.com/guide/components/fragments.html>

### Fragment生命周期
![fragment life](pic/1.png)

### Fragment与Activity生命周期相比
![activity life | fragment life](pic/2.png)

### 场景演示
##### 切换到该Activity
1. 11-29 14:26:35.095: D/AppListFragment(7649): onAttach
2. 11-29 14:26:35.095: D/AppListFragment(7649): onCreate
3. 11-29 14:26:35.095: D/AppListFragment(7649): onCreateView
4. 11-29 14:26:35.100: D/AppListFragment(7649): onActivityCreated
5. 11-29 14:26:35.120: D/AppListFragment(7649): onStart
6. 11-29 14:26:35.120: D/AppListFragment(7649): onResume

##### 屏幕灭掉
1. 11-29 14:27:35.185: D/AppListFragment(7649): onPause
2. 11-29 14:27:35.205: D/AppListFragment(7649): onSaveInstanceState
3. 11-29 14:27:35.205: D/AppListFragment(7649): onStop

##### 屏幕解锁
1. 11-29 14:33:13.240: D/AppListFragment(7649): onStart
2. 11-29 14:33:13.275: D/AppListFragment(7649): onResume

##### 切换到其它Fragment
1. 11-29 14:33:33.655: D/AppListFragment(7649): onPause
2. 11-29 14:33:33.655: D/AppListFragment(7649): onStop
3. 11-29 14:33:33.660: D/AppListFragment(7649): onDestroyView

##### 切换到本身Fragment
1. 11-29 14:33:55.820: D/AppListFragment(7649): onCreateView
2. 11-29 14:33:55.825: D/AppListFragment(7649): onActivityCreated
3. 11-29 14:33:55.825: D/AppListFragment(7649): onStart
4. 11-29 14:33:55.825: D/AppListFragment(7649): onResume

##### 回到桌面
1. 11-29 14:34:26.590: D/AppListFragment(7649): onPause
2. 11-29 14:34:26.880: D/AppListFragment(7649): onSaveInstanceState
3. 11-29 14:34:26.880: D/AppListFragment(7649): onStop

##### 回到应用
1. 11-29 14:36:51.940: D/AppListFragment(7649): onStart
2. 11-29 14:36:51.940: D/AppListFragment(7649): onResume

##### 退出应用
1. 11-29 14:37:03.020: D/AppListFragment(7649): onPause
2. 11-29 14:37:03.155: D/AppListFragment(7649): onStop
3. 11-29 14:37:03.155: D/AppListFragment(7649): onDestroyView
4. 11-29 14:37:03.165: D/AppListFragment(7649): onDestroy
5. 11-29 14:37:03.165: D/AppListFragment(7649): onDetach
