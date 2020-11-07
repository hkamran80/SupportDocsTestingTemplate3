# SupportDocs: DataSource
This is where SupportDocs gets its data!

<table>
    <tr>
        <td colspan="2">
            <strong>Your data source JSON url is:</strong> <a id="datasource_url" href="{{ datasource_url }}">{{ datasource_url }}</a>
        </td>
    </tr>
<tr>
    <td>
        How to use (SwiftUI)
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
<tr>
    <td>
        How to use (UIKit)
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
