# SupportDocs: DataSource
This is where SupportDocs gets its data!

**Your data source JSON url is:** | <a id="datasource_url" href="{{ datasource_url }}">{{ datasource_url }}</a>
| :-- | :-- |
| In your SwiftUI app, use it like this: `options.urls.dataSource = URL(string: "{{ datasource_url }}")!` |

<table>
    <tr>
        <td>
        **Your data source JSON url is:**
        </td>
        <td>
        <a id="datasource_url" href="{{ datasource_url }}">{{ datasource_url }}</a>
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
{{ table_of_contents }}

## Notes
Do **not** update this file (`README.md`) directly. Instead, update the file in `_scripts/README.md`.
