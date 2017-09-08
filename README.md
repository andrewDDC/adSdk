#聚合SDK说明
##sdk特点
1. 聚合sdk聚合了admob、facebook、adx、百度、mopub、俄罗斯VK等平台的banner、插屏、原生广告。
2. APP可根据自己的需求集成需要的平台，不需要的平台，则不继承对应SDK，也可以自由新增新的平台，扩展方便。
3. 可以自由设置平台的优先级、超时时间，确保最大可能拉取到广告，APP可以自己按照demo中的格式配置，如果有自己的server与sdk结合使用、
    加入分国家运营，则能使收益更加最大化。

1. ##一、banner使用说明（支持3中尺寸的banner（高度50、90、250方型））

    '/**
     * 不自动刷新
     * @param context
     * @param placementId 广告位ID
     * @param adSize banner尺寸
     */
public AdView(Context context,String placementId,AdSize adSize)
    /**
     * @param context
     * @param placementId 广告位ID
     * @param adSize banner尺寸
     * @param refreshInterval 刷新间隔时间
     */
public AdView(Context context,String placementId,AdSize adSize,int refreshInterval)
    /**
     * 设置监听
     * @param adListener
     */
public void setAdListener(AdListener adListener)
    /**
     * 触发广告load
     */
public void loadAd()
    /**
     * 释放资源、停止刷新
     */
public void destory()’

2. ##二、插屏使用说明
见InterstitialAd
3. ##三、原生使用说明

见NativeAd

