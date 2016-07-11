# NumberChange
#数字动态变化
##整数样式数字的变化:
    UICountingLabel *myLabel = [[UICountingLabel alloc] initWithFrame:CGRectMake(0, CGRectGetMaxY(self.label1.frame) +20, WIDTH, 45)];
    myLabel.textAlignment = NSTextAlignmentCenter;
    myLabel.font = [UIFont fontWithName:@"Avenir Next" size:48];
    myLabel.textColor = [UIColor colorWithRed:236/255.0 green:66/255.0 blue:43/255.0 alpha:1];
    [self.view addSubview:myLabel];
    //设置格式
    myLabel.format = @"%d";
    //设置变化范围及动画时间
    [myLabel countFrom:0 to:100 withDuration:2.0f];
##浮点数样式数字的变化:
    UICountingLabel *myLabel = [[UICountingLabel alloc] initWithFrame:CGRectMake(0, CGRectGetMaxY(self.label2.frame) +20, WIDTH, 45)];
    myLabel.textAlignment = NSTextAlignmentCenter;
    myLabel.font = [UIFont fontWithName:@"Avenir Next" size:48];
    myLabel.textColor = [UIColor colorWithRed:236/255.0 green:66/255.0 blue:43/255.0 alpha:1];
    [self.view addSubview:myLabel];
    //设置格式
    myLabel.format = @"%.2f";
    //设置变化范围及动画时间
    [myLabel countFrom:0.0 to:3198.23 withDuration:2.0f];
##带有千分位分隔符的浮点数样式:
    UICountingLabel *myLabel = [[UICountingLabel alloc] initWithFrame:CGRectMake(0, CGRectGetMaxY(self.label3.frame) +20, WIDTH, 45)];
    myLabel.textAlignment = NSTextAlignmentCenter;
    myLabel.font = [UIFont fontWithName:@"Avenir Next" size:48];
    myLabel.textColor = [UIColor colorWithRed:236/255.0 green:66/255.0 blue:43/255.0 alpha:1];
    [self.view addSubview:myLabel];
    //设置格式
    myLabel.format = @"%.2f";
    //设置分隔符样式
    myLabel.floatingPositiveFormat = @"###,##0.00";
    //设置变化范围及动画时间
    [myLabel countFrom:0.00 to:3048.64   withDuration:2.0f];
    
