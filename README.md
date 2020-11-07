# SupportDocs: DataSource
This is where SupportDocs gets its data!

**Your data source JSON url is:** | <a id="datasource_url" href="https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json</a>
| :-- | :-- |
| In your SwiftUI app, use it like this: `options.urls.dataSource = URL(string: "https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json")!` |

<table>
    <tr>
        <td>
        **Your data source JSON url is:**
        </td>
        <td>
        <a id="datasource_url" href="https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/aheze/SupportDocsTestingTemplate3/DataSource/_data/supportdocs_datasource.json</a>
        </td>
    </tr>
<tr>
<td>

  ```Swift
  struct ContentView: View {
      @State var supportDocsPresented = false
      let options: SupportOptions = SupportOptions(
          urls: .init(
            dataSource: URL(string: "https://raw.githubusercontent.com/hkamran80/SupportDocs/DataSource/_data/data.json")!,
            error404: URL(string: "https://google.com")!
          )
      )
      var body: some View {
          Button("Present") { self.supportDocsPresented = true }
          .sheet(isPresented: $supportDocsPresented) {
            
              /// pass it in here!
              SupportDocsView(options: options, isPresented: $supportDocsPresented)
          }
      }
  }
  ```
</td>
<td>

 ```Swift
  struct ContentView: View {
      @State var supportDocsPresented = false
      let options: SupportOptions = SupportOptions(
          urls: .init(
            dataSource: URL(string: "https://raw.githubusercontent.com/hkamran80/SupportDocs/DataSource/_data/data.json")!,
            error404: URL(string: "https://google.com")!
          )
      )
      var body: some View {
          Button("Present") { self.supportDocsPresented = true }
          .sheet(isPresented: $supportDocsPresented) {
            
              /// pass it in here!
              SupportDocsView(options: options, isPresented: $supportDocsPresented)
          }
      }
  }
  ```
</td>
</tr>
</table>

## Table of Contents
- [How to eat grilled cheese](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatGrilledCheese)
- [How to make spaghetti](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToMakeSpaghetti)
- [How to eat burritos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatBurritos)
- [How to eat tacos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatTacos)
- [How to eat nachos](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToEatNachos)
- [How to Prepare Ramen](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToPrepareRamen)
- [How to Cook Pizza](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-FastFood/HowToCookPizza)
- [Plum smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Plum)
- [Peach smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Peach)
- [Blueberry Smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Blueberry)
- [Red berry smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/RedBerries)
- [Apple smoothie](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Smoothies/Apple)
- [Buy cream boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyCreamBoba)
- [Buy blue boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyBlueBoba)
- [Buy orange boba](https://aheze.github.io/SupportDocsTestingTemplate3/Sample-Boba/BuyOrangeBoba)


## Notes
Do **not** update this file (`README.md`) directly. Instead, update the file in `_scripts/README.md`.