﻿```csdiff
 public class ShowOrders : UIControllerBase
{

    public readonly Models.Orders Orders = new Models.Orders();
    public ShowOrders()
    {
        From = Orders;

-       Handlers.Add(System.Windows.Forms.Keys.F8).Invokes += ShowOrders_Invokes;
+       Handlers.Add(System.Windows.Forms.Keys.F8).Invokes += e => Message.ShowWarning("Pressed F8");
    }

-   private void ShowOrders_Invokes(Firefly.Box.Advanced.HandlerInvokeEventArgs e)
-   {
-       Message.ShowWarning("Pressed F8");
-   }
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/HT0qxvVsKAM?list=PL1DEQjXG2xnIGbO3DlvFQjv-T0OXM81r-" frameborder="0" allowfullscreen></iframe>