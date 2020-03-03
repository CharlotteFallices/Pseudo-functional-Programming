# Pseudo-functional Programming
A mode of programming / 一个不成熟的设计模式
## 概述
先上一段代码:
```swift
public struct MakeLove{
  public var song:Song?//被添加的歌曲
  public var user:User?//用户的收藏歌单
  public func input(songIn:Song,userIn:User){
    song=songIn
    user=userIn
  }
  public func makeLove(){
    song.love=true
  }
  public logival/*逻辑判断单位*/ func isInLoving(){
    for i in 0..user.loving.length{
    //如果歌曲已经在Loving歌单内
      if user.loving[i].name==song.name{
        break
      }else{
        addToLoving()
      }
    }
  }
  public func addToLoving(){
    user.loving[user.loving.length]=song
  }
  public func outputSong()->Song{
    var tempSong=song
    song=nil
    return tempSong
  }
  public func outputUser()->User{
    var tempUser=user
    user=nil
    return tempUser
  }
}
```
现在还没想好要怎么描述,等我整理一下思路吧.
## License
This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
