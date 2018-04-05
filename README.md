# SFTextView
## 这是ios端一款带placeholder和字数限制的textview

### 使用方式如下：

```OC

    //初始化
    SFTextView *textView = [[SFTextView alloc] init];
    
    //设置基本属性
    textView.frame = CGRectMake(40, 40, 250, 300);
    textView.textColor = [UIColor redColor];
    textView.font = [UIFont systemFontOfSize:15];
    textView.layer.borderColor = [UIColor blackColor].CGColor;
    textView.layer.borderWidth = .5;
    
    //设置placeholder属性
    [textView setPlaceHolderAttr:@"请输入信息" textColor:[UIColor redColor] font:[UIFont systemFontOfSize:15]];
    
    //设置字数限制属性
    [textView setCharCountAttr:10 right:8 bottom:8 textColor:[UIColor redColor] font:[UIFont systemFontOfSize:15]];
    
    [self.view addSubview:textView];

```
