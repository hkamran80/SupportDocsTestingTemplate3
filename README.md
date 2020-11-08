# SupportDocs: DataSource
This is where SupportDocs gets its data!

<table>
  <tr>
    <td>
      <strong>Your data source JSON url is:
    </td>
  </tr>
  <tr>
    <td>
      <a id="datasource_url" href="https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json</a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      How to use (SwiftUI)
    </td>
  </tr>
  <tr>
  <td>
     
  ```Swift
  struct SwiftUIExampleView_MinimalCode: View {
    
      let options = SupportOptions(
          urls: .init(
              dataSource: URL(string: "https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json")!
          )
      )
    
      @State var supportDocsPresented = false
    
      var body: some View {
          VStack {
              Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
              .sheet(isPresented: $supportDocsPresented, content: {
                  SupportDocsView(options: options, isPresented: $supportDocsPresented)
              })
          }
      }
  }
  ```
  </td>
  </tr>
  
  <tr>
    <td>
      How to use (UIKit)
    </td>
  </tr>
  <tr>
  <td>
     
  ```Swift
  class UIKitExampleController_MinimalCode: UIViewController {
    
      /**
       Connect this inside the storyboard.
     
       This is just for demo purposes, so it's not connected yet.
       */
      @IBAction func presentButtonPressed(_ sender: Any) {
        
          var options = SupportOptions()
          options.urls.dataSource = URL(string: "https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json")!
        
          let supportDocsViewController = SupportDocsViewController(options: options)
          self.present(supportDocsViewController, animated: true, completion: nil)
      }
  }
  ```
  </td>
  </tr>
</table>

## Table of Contents
- [How to eat grilled cheese](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatGrilledCheese)- [How to eat grilled cheese](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatGrilledCheese)
- [How to make spaghetti](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToMakeSpaghetti)- [How to make spaghetti](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToMakeSpaghetti)
- [How to eat burritos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatBurritos)- [How to eat burritos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatBurritos)
- [How to eat tacos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatTacos)- [How to eat tacos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatTacos)
- [How to eat nachos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatNachos)- [How to eat nachos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatNachos)
- [How to Prepare Ramen](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToPrepareRamen)- [How to Prepare Ramen](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToPrepareRamen)
- [How to Cook Pizza](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToCookPizza)- [How to Cook Pizza](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToCookPizza)
- [Plum smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Plum)- [Plum smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Plum)
- [Peach smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Peach)- [Peach smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Peach)
- [Blueberry Smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Blueberry)- [Blueberry Smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Blueberry)
- [Red berry smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/RedBerries)- [Red berry smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/RedBerries)
- [Apple smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Apple)- [Apple smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Apple)
- [Buy cream boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyCreamBoba)- [Buy cream boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyCreamBoba)
- [Buy blue boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyBlueBoba)- [Buy blue boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyBlueBoba)
- [Buy orange boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyOrangeBoba)- [Buy orange boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyOrangeBoba)


## Notes
Do **not** update this file (`README.md`) directly. Instead, update the file in `_scripts/README.md`.