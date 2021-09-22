# How-to-set-style-to-badge-view
This repository contains sample for setting style to the badge view

This article explains how to set the style of the Xamarin.Forms badge view. 

By using BadgeSettings property we can customize and apply style to the badge view as like in below code snippet.

[XAML]
```
  <Style x:Key="BadgeViewStyle" TargetType="badge:SfBadgeView">
                <Setter Property="BadgeText">New User</Setter>
                <Setter Property="BadgeSettings">
                    <Setter.Value>
                        <badge:BadgeSetting BadgePosition="BottomRight" BackgroundColor="Green" CornerRadius="5"
                                     Offset="-15,-8"   BadgeType="None"   StrokeWidth="2" Stroke="Black"  BadgeIcon="Busy" BadgeAlignment="Start" />
                    </Setter.Value>
                </Setter>
            </Style>

        …

        <badge:SfBadgeView HorizontalOptions="Center" VerticalOptions="Center" Style="{StaticResource BadgeViewStyle}">
            <badge:SfBadgeView.Content>
                <Image Source="People_Circle1.png"   VerticalOptions="Center"
                           HorizontalOptions="Center"
                           HeightRequest="100" WidthRequest="100"/>
            </badge:SfBadgeView.Content>
        </badge:SfBadgeView>
````

![](Output.png)

## See also

[How can I customize the badge view position?](https://help.syncfusion.com/xamarin/badge-view/position-customization)

[How can I customize the badge in Xamarin.Forms SfBadgeView?](https://help.syncfusion.com/xamarin/badge-view/badge-customization)

[How can I add badge icon in badge view?](https://help.syncfusion.com/xamarin/badge-view/predefined-symbols)
