# WPF self binding
<code>DataContext="{Binding RelativeSource={RelativeSource Self}}</code>

# WPF ListView source binding
<code>ItemsSource="{Binding Entities, RelativeSource={RelativeSource FindAncestor, AncestorType={x:Type local:MainWindow}}}</code>

# WPF ListView Headers
https://wpf-tutorial.com/listview-control/listview-with-gridview/

# WPF sort ListView
https://docs.microsoft.com/en-us/dotnet/desktop/wpf/controls/how-to-sort-a-gridview-column-when-a-header-is-clicked?redirectedfrom=MSDN&view=netframeworkdesktop-4.8

# WPF ListView editable (not pretty)
<code>GridViewColumn Header="Name" Width="100"</code>

<code> GridViewColumn.CellTemplate </code>

<code> DataTemplate </code>

<code> TextBox Text="{Binding Name}" </code>

<code> /DataTemplate </code>

<code> /GridViewColumn.CellTemplate </code>

<code> /GridViewColumn </code>

# Serialize into XML

<code>System.Xml.Serialization</code>

<code>var writer = new XmlSerializer(typeof(List<Entity>))</code>

  <code>FileStream fs = File.Create("output.xml")</code>
  
  <code>writer.Serialize(fs, Entities)</code>
  
Tohle obalit do try-catch, catch nechat prázdnej
  
# ...
  
Zamyslet se jestli dělat edit a create v novým okně - dost otrava co se týče okna - nebo jestli to udělat vedle jako pár boxů a labelů + tlačítka na Update, Create New a Delete Selected. Možná to bude časově lepší - samotnej BE zabije půl hodiny určitě.
 
