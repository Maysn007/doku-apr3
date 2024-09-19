---
icon: code
date: '2024-09-19'
---

# Erstellung einer .NET MAUI App

 Folgende Schritte müssen bei der Erstellung einer `MAUI App` berücksichtigt werden.

1. Ordentlich Namen wählen [a-zA-Z0-9] (nicht `App`, `MauiApp`, etc.)
2. In den Abhängigkeiten werden die Pakete aktualisiert.
3. `Nuget`-Paket ´CommunityToolkit.mvvm` bei "Durchsuchen" suchen und anschließend installieren.
4. Kontrolle ob das Paket korrekt installiert worden ist.
5. Demo-Daten in den Dateien `Mainpage.xaml` und `Mainpage.xaml.cs` löschen und in der `Mainpage.xaml` ein `Grid` festlegen.
6. Erstellung eines Viewmodels namens: Neuer Ordner `Viewmodels` > In den Ordner eine neue Klasse z.B. `MainViewModel`.
7. Die Oberfläche (`Mainpage`) in der CodeBehind Datei (`Mainviewmodel.xaml.cs`) mit dem Viewmodel (`MainViewModel`) verbinden = `this.Bindingcontext = new MainViewModel;`.
8. Eine Eigenschaft (ObservableProperty) namens Title im MainViewModel erstellen und in der Oberfläche verwenden.
9. In der XAML-Datei (Mainpage.xaml) kann optional ein Namespace zum Order Viewmodels hinzugefügt werden und ein Datentyp für die Oberfläche festgelegt werden. Dadurch erhält man in Visual Studio passende Vorschläge (steht in der MainPage ganz oben, xmlns; und x:datatype)
10. Eine Methode kann im Viewodel hinzugefügt werden und der erstellte `Command` in der Oberfläche verwendet werden. 

![GeradeUngerade](/static/images/geradeungerade.png)