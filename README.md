# revise01_uiscrollview

##UIScrollview的属性
`
//设置scrollview在屏幕的大小
    self.myScroll = [[UIScrollView alloc] initWithFrame:[UIScreen mainScreen].bounds];
    //设置scorllview本身内容的大小
    self.myScroll.contentSize = CGSizeMake(size.width, 5*size.height);
    //设置delegate
    self.myScroll.delegate = self;
    //是否支持滑动到顶端
    self.myScroll.scrollsToTop = NO;
    //设置contentview与scrollview的边距(即scrollview的内边距)
    self.myScroll.contentInset = UIEdgeInsetsMake(0, 50, 50, 0);
    //设置偏移量
    self.myScroll.contentOffset = CGPointMake(50, 50);
    //设置是否反弹
    self.myScroll.bounces = NO;
    //设置是否分页
    self.myScroll.pagingEnabled = YES;
    //设置是否滚动
    self.myScroll.scrollEnabled = YES;
    //设置滚动条风格
    /**
     * UIScrollViewIndicatorStyleWhite   :白色
     * UIScrollViewIndicatorStyleDefault :默认(灰色)
     * UIScrollViewIndicatorStyleBlack   :黑色
     */
    self.myScroll.indicatorStyle = UIScrollViewIndicatorStyleWhite;
    //设置滚动条边缘
    self.myScroll.scrollIndicatorInsets = UIEdgeInsetsMake(0, 50, 0, 0);
    //控制是否显示水平方向的滚动条
    self.myScroll.showsHorizontalScrollIndicator = NO;
    //控制是否显示竖直方向的滚动条
    self.myScroll.showsVerticalScrollIndicator = YES;
    //设置scrollview缩放的范围
    self.myScroll.maximumZoomScale = 2.0f;//最大两倍
    self.myScroll.minimumZoomScale = 0.5f;
    //设置是否同时运动
    self.myScroll.directionalLockEnabled = YES;
`
