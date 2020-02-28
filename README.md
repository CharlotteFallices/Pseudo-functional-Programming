# Pseudo-functional Programming
A mode of programming / 一个不成熟的设计模式
## 概述
先上一段代码:
```swift
public struct MakeLove{
  public var song:Song?
  public func inputSong(songIn:Song){
    song=songIn
  }
  public func makeLove(){
    song.love=true
  }
  public func outputSong()->Song{
    var tempSong=song
    song=nil
    return tempSong
  }
}
```
现在还没想好要怎么描述,等我整理一下思路吧.
## License
This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
