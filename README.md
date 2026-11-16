<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-cartesia 1.3.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-cartesia.git", from: "1.3.0")
```

Products: `SwiftAICartesia`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Cartesia for Swift

`SwiftAICartesia` adds Cartesia to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/cartesia` and supports transcription and speech.

Provider guide with models, options, streaming and errors:

- [Cartesia](https://swiftaisdk.github.io/SwiftAISDK/providers/cartesia/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAICartesia` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAICartesia

let provider = try AIProviders.cartesia(configuration: CartesiaProviderSettings())
```

By default the provider reads `CARTESIA_API_KEY` from the environment; values set in `CartesiaProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-cartesia` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
