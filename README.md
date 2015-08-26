# RBOAuth2Manager
This Repo is a wrapper for AFOAuth2Manager.
It takes AFOAuth2Manager and all it's AFNetworking depencencies and builds a framework with them.

---

### Why
- AFOAuth2Manager doesn't has support for Carthage
- AFOAuth2Manager can't be compiled in Cocoapods witht he `use_frameworks!` configuration
- We needed it to be a `.framework` to integrate it easier in our SDK


### Compile
- Just execute the project and look for the `RBAuth2Manager.framework` in your system.
- Take that framework and use it wherever you want. All the classes inside it are public.


### Update Dependencies

- You have to do it manually. Download the AFOAuth2Manager source code and update it in this repo. Then do the same with all the dependencies.
- At the moment of writing this README, the only dependency is: `AFNetworking/NSURLConnection` that has also some sub-dependencies:
  - `AFNetworking/Serialization`
  - `AFNetworking/Reachability`
  - `AFNetworking/Security`
 
 