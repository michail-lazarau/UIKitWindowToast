# UIKitWindowToast

This can be utilized by using SPM.

This Swift Package give an opportunity to add a ToastView on the window of the app. The ToastView is added to the queue, retrieved and displayed immediately if it's 1st in the stack.

```swift
let toastManager = ToastManager(playPosition: ToastPosition(xAxisPosition: .center(), yAxisPosition: .top(constant: YAxisPosition.navigationBarIndent)),
                                prePosition: ToastPosition(xAxisPosition: .center(), yAxisPosition: .top(constant: YAxisPosition.notchIndent)),
                                postPosition: ToastPosition(xAxisPosition: .center(), yAxisPosition: .top(constant: YAxisPosition.notchIndent)))
        toastPresenter.enqueueToastForPresentation(toast: DefaultToastView(), toastManager: toastManager)
```

![Simulator Screen Recording - iPhone 14 Pro - 2023-02-24 at 17 04 24](https://user-images.githubusercontent.com/71278978/221198148-cdd9e838-d759-4839-97b3-2f91d1c240d9.gif)
