# SwiftUI_CustomPageControl


```swift


struct CustomPageControl: UIViewRepresentable {

    
    var currentPage: Int = 0
    var numberOfPages: Int
    
    func makeUIView(context: UIViewRepresentableContext<CustomPageControl>) -> UIPageControl {
        let page: UIPageControl = UIPageControl()
        page.currentPageIndicatorTintColor = .black
        page.numberOfPages = numberOfPages
        page.pageIndicatorTintColor = .gray
        return page
    }
    
    func updateUIView(_ uiView: UIPageControl, context: Context) {
        uiView.currentPage = currentPage
    }
    
}


```
