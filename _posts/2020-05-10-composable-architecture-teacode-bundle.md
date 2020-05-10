I've been working with The Composable Architecture from pointfreeco for several weeks now and love it. The best thing for me is that it has a strong opinion on how to set up an app. But this also means that there is a b it of boiler plate that you end up adding to each view. You need a **state** and **action** enum. Quite often there is a **reducer** and the **init()** sets up the **store** the same way each time.

The whole point of TCA is that it is composable so you end up with a lot of **states, actions, stores, and reducers** throughout your code.
so I made some TeaCode expanders to help out. Now that TCA has had it's first release I've adapted my expanders and am sharing them [here](/assets/ComposableArchitecture.tcbundle.zip)
