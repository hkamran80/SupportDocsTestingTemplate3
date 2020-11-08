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
- [How to eat grilled cheese](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatGrilledCheese)["edit"](support_document['url'])
- [How to make spaghetti](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToMakeSpaghetti)["edit"](support_document['url'])
- [How to eat burritos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatBurritos)["edit"](support_document['url'])
- [How to eat tacos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatTacos)["edit"](support_document['url'])
- [How to eat nachos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatNachos)["edit"](support_document['url'])
- [How to Prepare Ramen](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToPrepareRamen)["edit"](support_document['url'])
- [How to Cook Pizza](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToCookPizza)["edit"](support_document['url'])
- [Plum smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Plum)["edit"](support_document['url'])
- [Peach smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Peach)["edit"](support_document['url'])
- [Blueberry Smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Blueberry)["edit"](support_document['url'])
- [Red berry smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/RedBerries)["edit"](support_document['url'])
- [Apple smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Apple)["edit"](support_document['url'])
- [Buy cream boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyCreamBoba)["edit"](support_document['url'])
- [Buy blue boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyBlueBoba)["edit"](support_document['url'])
- [Buy orange boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyOrangeBoba)["edit"](support_document['url'])


## Notes
Do **not** update this file (`README.md`) directly. Instead, update the file in `_scripts/README.md`.