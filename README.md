# glow-test-ios

- 在HomeVc项目基础上继续开发。
- Main.storyboard里面已经提供了HomeViewController和三个作为 child view controller的 TodayViewController/AnalysisViewController/ResourcesViewController，HomeViewController的view里面已经添加了蓝色背景的’Home Top Part’和 有三个Segments的UISegmentedControl控件。
- 需要实现把TodayViewController/AnalysisViewController/ResourcesViewController三个view controller的内容显示到HomeViewController的segmented control下方。segmented control 默认选中Today，下方默认显示TodayViewController的view。点击segmented control的Analysis，下方会显示AnalysisViewController的view。点击segmented control的Resources，下方会显示为ResourcesViewController的view。
- 需要实现左右滑动的切换效果。如果当前显示了TodayViewController，用户手指向右滑动会bounce回到TodayViewController，用户手指向左滑动会切换显示到AnalysisViewController的view，同时segemented control会高亮ANALYSIS。如果当前显示的是AnalysisViewController的view，则用户手指向右滑到TodayViewController或者用户手指向左滑到ResourcesViewConroller的view，滑动完成后同时更新segmented control的高亮segment。
- 需要实现上下滑动时候隐藏和显示Home Top Part，同时把segmented control移动到紧贴navigation bar的位置，或者默认位置。Home Top Part所在view的默认高度是220points。当前显示的child view controller在用户手指向上滑动的时候，如果已经看不到child view controller的前三行cell，则隐藏Home Top Part，同时segmented control移动到紧贴navigation bar的位置。当前显示的child view controller在用户手指向下滑动的时候，如果已经滑动到顶，则显示Home Top Part，同时segemented control移动到默认位置。
- 根据需要自行修改swift文件和storyboard文件。
