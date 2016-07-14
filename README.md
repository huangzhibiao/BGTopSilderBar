# BGTopSilderBar   
#高仿网易新闻,斗鱼的顶部滑动导航栏   
##使用非常方便，几行代码搞定：   
/**   
初始化BGTopSilderBar   
*/   
-(void)initSilderBar{   
BGTopSilderBar* silder = [[BGTopSilderBar alloc] initWithFrame:CGRectMake(0,20,screenW, 50)];   
//silder.contentCollectionView = _collectView;//_collectView必须要在前面初始化,不然这里值为nil   
silder.contentCollectionView = _scrollView;//_scrollView必须要在前面初始化,不然这里值为nil   
_silderBar = silder;   
[self.view addSubview:silder];   
}   
##特别标注：    
这里可以使用UICollectionView和UIScrollView来做各各页面，此默认使用UIScrollView来添加不同的UIViewController来做，   
而UICollectionView是通过BGTopSilderBarCell来做个个页面,看自己习惯哪一种.
