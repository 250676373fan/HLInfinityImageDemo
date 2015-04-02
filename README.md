# HLInfinityImageDemo
a loop scrollview and easy to use

example:
  NSArray *imgArray = @[
                        @"1.png",
                        [UIImage imageNamed:"2.png"],
                        [NSURL URLWithString:@""],
                        ];
    HLInfinityImageView * infinityView = [HLInfinityImageView infinityScrollViewWithBuilder:^(HLInfinityImageViewBuilder *builder) {
        builder.frame = self.view.bounds;
        builder.imageArray = imgArray;
        builder.interval = 2.5;
    }];
    [self.view addSubview:infinityView];
