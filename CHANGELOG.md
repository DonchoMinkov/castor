# Changelog

## [2.0.0](https://github.com/DonchoMinkov/castor/compare/v2.5.0...v2.0.0) (2026-11-12)


### ⚠ BREAKING CHANGES

* Castor 1.x configuration must be migrated to the cast and servers sections. See the [1.x → 2.0 migration guide](https://github.com/stupside/castor/blob/main/migrations/1.x-to-2.0.md).

### Features

* add Roku cast target ([#50](https://github.com/DonchoMinkov/castor/issues/50)) ([9af2b53](https://github.com/DonchoMinkov/castor/commit/9af2b531ceb5ecaf55f36858a3ffb985b55b323e))
* **api:** drive a castor server for the renderers on the client's network ([0b94ae0](https://github.com/DonchoMinkov/castor/commit/0b94ae0de9b0da1892a8fc0fb7114930d8bc6b54))
* **api:** hold every message to the contract both ways, with protovalidate and CEL rules ([35ea3c4](https://github.com/DonchoMinkov/castor/commit/35ea3c4e9c5d75297e11942b0d5554a502b49578))
* **api:** log the address of the device a client lends, which the contract sends for that ([520eec2](https://github.com/DonchoMinkov/castor/commit/520eec217f2ff8a29dcbb80edb40aea0d9e86c7c))
* **api:** make the server the media server, which TVs fetch from and which outlives its client ([b1eccf0](https://github.com/DonchoMinkov/castor/commit/b1eccf067e9173115bdaba364dfa438ee7b128d8))
* **api:** serve casts behind the contract, driving renderers only through a client ([ff1e30b](https://github.com/DonchoMinkov/castor/commit/ff1e30bd875eeff27bdcd4821d99f546f59086bb))
* **api:** state the cast contract in protobuf, generated with buf for Connect ([01bd3c1](https://github.com/DonchoMinkov/castor/commit/01bd3c172490552d44ac9d6202fe619a80b079bb))
* **app:** add the web client ([cd0932b](https://github.com/DonchoMinkov/castor/commit/cd0932b68dcfc478b2b537ab747a0e9fa216fdcb))
* **app:** expose manual targets and per-cast playback options ([c82db80](https://github.com/DonchoMinkov/castor/commit/c82db8038ac6157e6657e9d45a31d9462e1f4b92))
* **app:** rebuild the admin on StyleX ([c0bb1dd](https://github.com/DonchoMinkov/castor/commit/c0bb1dd3df2a0b4bac147cae2caa6fef197e50a4))
* **cast:** begin a cast at a position ([754ef18](https://github.com/DonchoMinkov/castor/commit/754ef18743916f3b7250c88fc10452fe572eaadc))
* **cast:** bind the ceiling to the hand-off, reject what cannot be fetched, and test the read against a hostile origin ([fd46c0e](https://github.com/DonchoMinkov/castor/commit/fd46c0efe5b6aa6a93c00eca1f48bd2c4be9b7ef))
* **cast:** follow the device's link while it plays ([abf1428](https://github.com/DonchoMinkov/castor/commit/abf14280b88afcb02706d4aab13e203eeaaf432b))
* **cast:** go back to a better ranked link once the cast plays well ([13e5d93](https://github.com/DonchoMinkov/castor/commit/13e5d932b2738e2d91a8754c670cedf55968d81b))
* **cast:** keep the machine from idling to sleep while casting ([99119c6](https://github.com/DonchoMinkov/castor/commit/99119c6888a698290b2c6e7dbc18c81b2520b74b))
* **cast:** let the device play out what it took before stopping ([b525cb7](https://github.com/DonchoMinkov/castor/commit/b525cb7f2b7c4ab64035d6e221e7f0fb8c5385e7))
* **cast:** let the interactive cast run without a configured device ([34f5e89](https://github.com/DonchoMinkov/castor/commit/34f5e8948679e2fe4da79c6c6ef9454fd9717856))
* **cast:** negotiate subtitle delivery and own backend lifecycles ([77a876b](https://github.com/DonchoMinkov/castor/commit/77a876b3000d9574c594c23c98aab2ba1b230851))
* **cast:** pass a source's HLS captions to the device and play the audio language asked ([f8eb7cb](https://github.com/DonchoMinkov/castor/commit/f8eb7cb7f4bbc96dae8ebe6ca485e7272b701873))
* **cast:** pause, resume and seek a cast through the API ([c3ade03](https://github.com/DonchoMinkov/castor/commit/c3ade03b2cadd8830ceb0b83cc909e8f8454da0d))
* **cast:** replace the cast playing on a busy device ([7932455](https://github.com/DonchoMinkov/castor/commit/7932455538e4205ccef582ec57f4f2a3cc9d5446))
* **cast:** resolve a device by id and refuse an ambiguous name ([02bdd84](https://github.com/DonchoMinkov/castor/commit/02bdd84a18ff9f51cdaf031cc5c515d1c97dbc98))
* **cast:** show the captions a stream is given with ([4120c05](https://github.com/DonchoMinkov/castor/commit/4120c053ccc4b3b763f8cef2453f8e1b9720e9b8))
* **cast:** start a device once the read holds thirty seconds ([03b8dd4](https://github.com/DonchoMinkov/castor/commit/03b8dd4aada62bcaa6940d1f51c6d9967b5ffaae))
* **cast:** surround audio and compiler-isolated device strategies ([bed47e9](https://github.com/DonchoMinkov/castor/commit/bed47e940915f2a163f9c9cef635fbfa506d96e0))
* **cast:** tell a Turns port each attempt and revision a cast takes ([53c558b](https://github.com/DonchoMinkov/castor/commit/53c558bf519cd2c1a610787f4d88ff9a326eed0c))
* **cli:** also write log lines to castor.log in the user cache directory ([1cc5f25](https://github.com/DonchoMinkov/castor/commit/1cc5f2563d6d5730b1456a2b8d08596a2334fb37))
* **cli:** compose the scraping service ([cbf8c1c](https://github.com/DonchoMinkov/castor/commit/cbf8c1cbc0c066ce3ad1c6531ff9f67e21f3a74c))
* **cli:** split castor api-server from castor media-server ([7a14f2f](https://github.com/DonchoMinkov/castor/commit/7a14f2fda8614f0fa2cf92bf5541671974e30b79))
* **cmd:** cast through the API, served in process or by castor api server ([44fe6a6](https://github.com/DonchoMinkov/castor/commit/44fe6a6f5a66890c8b6c5eae54c4564d18b24c71))
* **cmd:** hold the client's log lines back while a screen is up, and write them after ([37efe53](https://github.com/DonchoMinkov/castor/commit/37efe5376c864df52a7b56ae9dd6f72a6dae1999))
* **cmd:** show a cast's warnings without --debug, and the embedded engine's own lines with it ([43b1ab8](https://github.com/DonchoMinkov/castor/commit/43b1ab88dbf95b08d23de6e72a4554994b4af23c))
* **config:** allow custom FFmpeg tool paths ([22fa98e](https://github.com/DonchoMinkov/castor/commit/22fa98ea391e4bd0906de371dadf59484446c0ce))
* **config:** refuse a subtitle language that is neither a BCP-47 tag nor auto ([a2d1f3b](https://github.com/DonchoMinkov/castor/commit/a2d1f3b15a2ad9cabafd2a45f6b1ee49fdf6d9ea))
* **device:** connect by pinned host, skipping discovery ([d16351e](https://github.com/DonchoMinkov/castor/commit/d16351e171183e0f048744c30fbf6442dadcce88)), closes [#24](https://github.com/DonchoMinkov/castor/issues/24)
* **device:** follow the devices as they come and go ([c616617](https://github.com/DonchoMinkov/castor/commit/c6166177dbf16f28d09c9912bb450f4a9f221508))
* **device:** pause and resume the lent device ([16067e5](https://github.com/DonchoMinkov/castor/commit/16067e5a546f61342f0e56fcce00393088e78476))
* **device:** report the device's position and its viewer's pause ([e6a5e82](https://github.com/DonchoMinkov/castor/commit/e6a5e82970fbd809278457e9a97bc0ccfb6986dd))
* discover chromecast devices via mDNS ([e6c419f](https://github.com/DonchoMinkov/castor/commit/e6c419fa1192bb3818c3c3674fb0986c16002b56))
* discover Chromecast devices via mDNS ([ee41e6f](https://github.com/DonchoMinkov/castor/commit/ee41e6f2e7a1c512b400e7cb4f5ba53dccec8d59))
* **dlna:** seek within the stream castor serves ([c55fbc7](https://github.com/DonchoMinkov/castor/commit/c55fbc7593d7670827ce39017ec4071627007a27))
* **docker:** run media-server and api-server as separate compose services ([e04ad9f](https://github.com/DonchoMinkov/castor/commit/e04ad9f98109c86059bf56208cb656ff6ce50d8b))
* **docker:** run the scraping service ([6b20800](https://github.com/DonchoMinkov/castor/commit/6b20800fc5d4653ab0c00a72c89f93378690382a))
* drop short streams when ranking candidates ([46bb4b7](https://github.com/DonchoMinkov/castor/commit/46bb4b707d111505e7fd8e46c266fcf2de0f6a51))
* **encoding:** encode on MediaCodec where the host declares it ([678e713](https://github.com/DonchoMinkov/castor/commit/678e713d39453c6397962a23d420ebeedd887cbb))
* **extract:** disable site isolation to capture cross-origin iframe requests ([d851f54](https://github.com/DonchoMinkov/castor/commit/d851f54cb43a94deae1c54410ffd73d14fc6d18b))
* **ffmpeg:** read a demuxed program as two inputs ([2039f1d](https://github.com/DonchoMinkov/castor/commit/2039f1d2038d79fc59c8eb0767e7b82e547e0297))
* **ffmpeg:** use private named pipes for Windows side outputs ([9a70573](https://github.com/DonchoMinkov/castor/commit/9a70573ee8796b551323a2b7b447b232238cdf4c))
* **health:** hold a device its read falls behind instead of letting it run dry ([2dd5262](https://github.com/DonchoMinkov/castor/commit/2dd52625e262c88064d5cadf29b96d6bce0a6ace))
* **health:** start a cast on a short cushion and judge it by its whole fill ([4db780c](https://github.com/DonchoMinkov/castor/commit/4db780caa4d29f4c1dfb72542d3506d2df02b1b2))
* keep castor's own timeline, slice the tree by feature, and read media with maintained libraries ([cfdc78a](https://github.com/DonchoMinkov/castor/commit/cfdc78a19ad7500f913579e6bf87301376fb2315))
* live-edge pacing at realtime with no burst ([551ddf0](https://github.com/DonchoMinkov/castor/commit/551ddf054c8ab420197878bad99f1bcc8e8425e9))
* **log:** export logs over OTLP and tag every line with its cast id ([6aa0f55](https://github.com/DonchoMinkov/castor/commit/6aa0f551e1a0b84a7eb772480d3e7ebebc94dc40))
* **media:** let one program span two renditions ([6055517](https://github.com/DonchoMinkov/castor/commit/6055517517adcb88b2496545376352e583848f9a))
* **picker:** quit on q at once, without a confirmation dialog ([959e0ea](https://github.com/DonchoMinkov/castor/commit/959e0eaa880b0f17f362f251d2f9a36dcc156d97))
* **rank:** rank links by the language of their sound first ([1992d9c](https://github.com/DonchoMinkov/castor/commit/1992d9c09a19e248e3a83828fdb3e08c1bda7bbe))
* **release:** give the npm launcher search keywords ([#77](https://github.com/DonchoMinkov/castor/issues/77)) ([6888ed7](https://github.com/DonchoMinkov/castor/commit/6888ed7a4c466d924ecbc5a8824b76a334d18f4d))
* **release:** publish the cli to npm through trusted publishing ([99c3403](https://github.com/DonchoMinkov/castor/commit/99c3403a5cc1eed4b0d6fbca463565383b01d98b))
* **release:** ship the project docs in every npm package ([c5f7b45](https://github.com/DonchoMinkov/castor/commit/c5f7b4574495b245d820b14a62702b05c83b2fa5))
* **release:** ship windows builds, and carry ffmpeg's side feeds over loopback ([#66](https://github.com/DonchoMinkov/castor/issues/66)) ([f3cf5ab](https://github.com/DonchoMinkov/castor/commit/f3cf5ab406592c4eaf175d9e337d504b8f164e6c)), closes [#61](https://github.com/DonchoMinkov/castor/issues/61)
* replay real browser headers to ffmpeg and ffprobe ([9e386f0](https://github.com/DonchoMinkov/castor/commit/9e386f028c183a1eec913a047c877ae3b7f901b8))
* **resolve:** detect a source only a lenient reader can open ([af3ec35](https://github.com/DonchoMinkov/castor/commit/af3ec35ff04d12c89390a89d1d85b6a89b37191b))
* **resolve:** keep the chosen variant's audio rendition ([3e4af34](https://github.com/DonchoMinkov/castor/commit/3e4af34bec7a13ea37a0a375baba45fda07f6eee))
* **scraping:** add the resolver service ([e4f6d08](https://github.com/DonchoMinkov/castor/commit/e4f6d08ed87091ff65e2938b96889d90bc4c6e05))
* **scraping:** improve player and iframe stream discovery ([08372b5](https://github.com/DonchoMinkov/castor/commit/08372b55f19b48eb90c30de8d28e2dac2764f2a5))
* **settings:** read the user's config directory, then the working directory's ([dc73421](https://github.com/DonchoMinkov/castor/commit/dc7342159166cfa6cc9298208f08f6cd47c10148))
* show cast target device in browse header ([0ae5f60](https://github.com/DonchoMinkov/castor/commit/0ae5f60269284bd2e753c81317838dce20530d32))
* show selected media details on playback devices ([9269a6d](https://github.com/DonchoMinkov/castor/commit/9269a6d9907466f928e682eb523f84449bc4a736))
* **source:** identify a master by its own tags, and bind the height cap to the copy ([d755b90](https://github.com/DonchoMinkov/castor/commit/d755b9092e4fe7c13641ce62bcec3a113e58eaa5))
* **source:** read HLS segments ahead of ffmpeg, several at once ([91ee224](https://github.com/DonchoMinkov/castor/commit/91ee224d94832cc2302eadae7487d7013b9dc6d9))
* **source:** unwrap PNG segments for inspection and playback ([6533f04](https://github.com/DonchoMinkov/castor/commit/6533f04a9ca9c90e2e28c93fc07bbb33bf4b406e)), closes [#68](https://github.com/DonchoMinkov/castor/issues/68)
* **telemetry:** namespace OTel names and make logs say why ([59432f5](https://github.com/DonchoMinkov/castor/commit/59432f5d4cddf38708cd41f99361766632963ce6))
* **telemetry:** record state machines as one span per state ([88d4ef1](https://github.com/DonchoMinkov/castor/commit/88d4ef181e26119c159753dc07e5c93a1d957ad4))
* **telemetry:** second-scale duration buckets, semconv 1.43 and service version ([2d74882](https://github.com/DonchoMinkov/castor/commit/2d7488270f87a77c9606935135b2a232aab084e3))
* update docker run instruction with working proxy ([aae56e4](https://github.com/DonchoMinkov/castor/commit/aae56e491985605bbdf669d6b75ba7bf0ac57cea))


### Bug Fixes

* **api:** bound concurrent device commands ([dddc689](https://github.com/DonchoMinkov/castor/commit/dddc689f0d438efcac0b201e2db56c1d31adf74a))
* **api:** cancel target discovery and protect cast snapshots ([5ef9c76](https://github.com/DonchoMinkov/castor/commit/5ef9c763a41a1e9c6a1b0ec76ed88774e12d24eb))
* **api:** cancel watch log forwarding ([e6306df](https://github.com/DonchoMinkov/castor/commit/e6306df6be0d27e56235ba3ff2f8147dab2e71db))
* **api:** end a cast at once when it needs a device whose client has left ([95587d7](https://github.com/DonchoMinkov/castor/commit/95587d71baeddff75656bfb844b97a7565a7e4cb))
* **api:** give castor api server's shutdown its grace before it exits ([60db9e8](https://github.com/DonchoMinkov/castor/commit/60db9e89297827927957da8adab6c7e82a3ab439))
* **api:** leave a cancelled extraction or ranking to connect's own code ([618959f](https://github.com/DonchoMinkov/castor/commit/618959f1147789429c188c58cb0484c8cf3516c0))
* **api:** let only http and https links reach the server's browser and readers ([99b07de](https://github.com/DonchoMinkov/castor/commit/99b07dedd5cbedbaabbc747af91c868d46d517e2))
* **api:** refuse a cast that leaves its delivery unstated ([a39d7ac](https://github.com/DonchoMinkov/castor/commit/a39d7acf0dda9ba9f6038ece18cefea246f91d31))
* **api:** refuse a device that answers connect without its capabilities ([88890c3](https://github.com/DonchoMinkov/castor/commit/88890c3507c5e141e1ce2164018ad094e655c61e))
* **api:** reject reused device command IDs ([3e1cb29](https://github.com/DonchoMinkov/castor/commit/3e1cb290215087c2a05f871edd196c9f6b976483))
* **api:** send on the Drive stream from its handler alone, each send bounded by its call ([aed4130](https://github.com/DonchoMinkov/castor/commit/aed41302c8508777ec86cfcbdff3c0f767681fa7))
* **api:** stop relaying a delivery's port once its listener closes ([f3a2b17](https://github.com/DonchoMinkov/castor/commit/f3a2b17bcdacfc671c0f16442fec660ab3992bf2))
* **app:** authorize server actions and propagate telemetry ([c5b7d55](https://github.com/DonchoMinkov/castor/commit/c5b7d5515b62f45e3e8b0c624cc017748e717a01))
* **app:** isolate watch credentials and cancel upstream streams ([a40cde5](https://github.com/DonchoMinkov/castor/commit/a40cde5697e3bab652dbf22e4a6fe1a8adf149b3))
* apply HLS-only ffmpeg input flags to HLS sources only ([6363a89](https://github.com/DonchoMinkov/castor/commit/6363a89dadc25cf12027ad9656fe67da75ad52ee))
* **app:** model cast watch outcomes as exclusive states ([b268e46](https://github.com/DonchoMinkov/castor/commit/b268e46d65513d5625990f290161c98a9e277282))
* **app:** recover device discovery and make cast controls resilient ([9d2381a](https://github.com/DonchoMinkov/castor/commit/9d2381a48a6ad39cecba44a3748b57a8ce0f9314))
* avoid VideoToolbox SEI failure on re-encode ([407e505](https://github.com/DonchoMinkov/castor/commit/407e5058ef36f5f6667f42aed3169eb7cc05c0ff))
* **cast:** blame a delivery silent over castor's proven buffer on the delivery, not the source ([8692a71](https://github.com/DonchoMinkov/castor/commit/8692a715c9be6e9f720dc9274c6dd538985c2b54))
* **cast:** count what the encoders made where they read the buffer ([77ff94a](https://github.com/DonchoMinkov/castor/commit/77ff94aaf12d625138948d132d38886b5cdc0aa6))
* **cast:** end a playing cast whose renderer has had nothing to play for the stall window ([81bf059](https://github.com/DonchoMinkov/castor/commit/81bf059d33a35fc9e7837d98c862315aa0fac02b))
* **cast:** fail a cast whose device ran out of media before the read finished ([f11a2da](https://github.com/DonchoMinkov/castor/commit/f11a2da42fe7564d4da1285bf41cec93d9b216c2))
* **cast:** give up on a delivery whose producer never writes its first artifact ([80b2739](https://github.com/DonchoMinkov/castor/commit/80b273941c74c33b3813a53fbe6e02bf3bdc73e9))
* **cast:** hear sound where the source declares or requires it, and say when subtitles are skipped ([6781cb5](https://github.com/DonchoMinkov/castor/commit/6781cb52dbce8d142902b0981fa8e1ad12ea71e7))
* **cast:** honor ordered playback language preferences ([c10249b](https://github.com/DonchoMinkov/castor/commit/c10249b5504d93630eaf2d48628f64411442238e))
* **cast:** join the source read before teardown releases what it reads from ([09972a2](https://github.com/DonchoMinkov/castor/commit/09972a24c3384e5c57b1f7fa135fe767cfd4e0aa))
* **cast:** judge a producer's growth against playback pace, not since the cast began ([fa41f6d](https://github.com/DonchoMinkov/castor/commit/fa41f6d626d052956dda5afc052aed008811e6ce))
* **cast:** let web receivers read the HLS castor makes ([e502197](https://github.com/DonchoMinkov/castor/commit/e50219797f65ce0510237439a0885de1d8252e3b))
* **cast:** log a failed lighter rendition by the link castor read, not the rung's missing URL ([1f24dd8](https://github.com/DonchoMinkov/castor/commit/1f24dd80bc1af82807deae25fa4be7c8605912ba))
* **cast:** make an encode that fails or hangs again in software ([af17bea](https://github.com/DonchoMinkov/castor/commit/af17beaa075414911a4fa1dab21bf6cb580c84a6))
* **cast:** move to the next link when castor cannot read a timeline it follows ([7fc34ad](https://github.com/DonchoMinkov/castor/commit/7fc34adc934f548468927e6a0b1b6158d40cd371))
* **cast:** name a device that ran dry starved ([8ef27d2](https://github.com/DonchoMinkov/castor/commit/8ef27d27b541aff5f561691d0365066e9a8619d6))
* **cast:** name why a device refused, and drop the prose behind it ([98848f7](https://github.com/DonchoMinkov/castor/commit/98848f7b7ba193c7378395553259b4326a112425))
* **cast:** return error from BuildPlan instead of panicking for unknown device type ([5f50298](https://github.com/DonchoMinkov/castor/commit/5f502988fea5dc01b0d1ac849b12c4d9bd5f3955))
* **cast:** serve instead only when the renderer was handed the source ([5d30281](https://github.com/DonchoMinkov/castor/commit/5d302815df2691874436e219f8416d2d27c88cc8))
* **cast:** serve sources that need request headers ([#54](https://github.com/DonchoMinkov/castor/issues/54)) ([e6d6880](https://github.com/DonchoMinkov/castor/commit/e6d6880ee39611fdf3b7d59ebc0a6499009b3743))
* **cast:** transcribe only a read sure to carry sound ([ff9cdd8](https://github.com/DonchoMinkov/castor/commit/ff9cdd848cef9b76b9ada1433bf9d0fccee63049))
* **cast:** validate served media and measure HLS renditions ([65a373c](https://github.com/DonchoMinkov/castor/commit/65a373c867ba77cd2d235b56ae1afa0e124bd06b))
* **chromecast:** cancel blocked writes ([3cf18a0](https://github.com/DonchoMinkov/castor/commit/3cf18a0ea65f050168dec6504845b4c883da2fc1))
* **chromecast:** end the cast as gone when the Cast connection drops ([8b1dcee](https://github.com/DonchoMinkov/castor/commit/8b1dcee20204858f43f6e8f8d20be2ee3093a521))
* **chromecast:** leave a newer cast playing when an earlier load is cancelled ([e415d9a](https://github.com/DonchoMinkov/castor/commit/e415d9a2dbf77312cc35378aa07b542dced6035b))
* **chromecast:** match LOAD status to the requested stream ([5c2c253](https://github.com/DonchoMinkov/castor/commit/5c2c25373ea5e9cd975e98c15c6fa3530cb81861))
* **chromecast:** reject LOAD replies without media status ([d2c0a33](https://github.com/DonchoMinkov/castor/commit/d2c0a33ba16eb82b8a32140c307a602e0c407bfd))
* **chromecast:** say when a playlist is cut into fMP4 ([46091f6](https://github.com/DonchoMinkov/castor/commit/46091f6894833c8bac592d9e6105151f0e925873))
* **ci:** restore release PR checks ([ccaec02](https://github.com/DonchoMinkov/castor/commit/ccaec0288d6ba77e694d140eee713649549eae8d))
* **ci:** update Staticcheck for the Go toolchain ([4dfe4fb](https://github.com/DonchoMinkov/castor/commit/4dfe4fbb41dc1d6e81192789ddaab867c4367716))
* clear quarantine xattr in cask postflight ([91994f6](https://github.com/DonchoMinkov/castor/commit/91994f6f57388e675129990051c954fba46b42bc))
* clear quarantine xattr in cask postflight so castor runs after brew install ([4f07f62](https://github.com/DonchoMinkov/castor/commit/4f07f62d9cc252ccc39defbe356ebd52448836bd)), closes [#17](https://github.com/DonchoMinkov/castor/issues/17)
* **client:** leave the drive when an answer to the server is lost ([00e6c54](https://github.com/DonchoMinkov/castor/commit/00e6c540aa59a2ccfbe3344b11bf92c4736865ab))
* **client:** lend the LAN only the server's relay route, never its API ([c011b77](https://github.com/DonchoMinkov/castor/commit/c011b77eab524acf76b49bf46be9cfc508291296))
* **client:** open the LAN relay for the first play that needs one, never to close it ([d88d3a5](https://github.com/DonchoMinkov/castor/commit/d88d3a568b193e1be215acad8859d9b5c3cfd04d))
* **cli:** isolate genre drafts and discard stale browse results ([5cbe5a2](https://github.com/DonchoMinkov/castor/commit/5cbe5a20cd2065079fd973b91b343f910283ae61))
* **cli:** keep forwarding buffered logs ([5b05612](https://github.com/DonchoMinkov/castor/commit/5b056122612cb917a16e02549631004c402d2f1d))
* **cli:** load only configuration needed by each cast action ([ef7acba](https://github.com/DonchoMinkov/castor/commit/ef7acba9c9f0e82d79ac508ba5be87178dc19888))
* **cli:** preserve grouped log redaction while holding output ([1e91f5f](https://github.com/DonchoMinkov/castor/commit/1e91f5f5ad8adb7643eaa53739ad7d497e69db3c))
* **cli:** refuse to start when the log file cannot be written ([0d7070a](https://github.com/DonchoMinkov/castor/commit/0d7070a3a386054af5f2539fdf25ed874bd6979e))
* **cli:** require cast arguments and preserve configured scan endpoints ([10c3cd3](https://github.com/DonchoMinkov/castor/commit/10c3cd3111041fec13a7797ed51d7475ef074d34))
* **cli:** stop casts when their status watch breaks ([ccaa503](https://github.com/DonchoMinkov/castor/commit/ccaa503c24a7c026117fdf520088afd6232d68ad))
* **cli:** stop q quitting the drilldown and tidy the browse loop ([a8362a3](https://github.com/DonchoMinkov/castor/commit/a8362a3cc201b687494b7328a87a06f49f042656))
* **cmd:** propagate picked device's type and host, not just name ([eff8f07](https://github.com/DonchoMinkov/castor/commit/eff8f0786b384720418e635758f98a9bbfe50f38))
* **cmd:** stop a cast only on Ctrl+C, not when its watch ends ([a321d39](https://github.com/DonchoMinkov/castor/commit/a321d39d7ff77acf1479fb7febe4417e00e927ba))
* **cmd:** stop the cast and release the drive whatever ended its watch ([f7a34d4](https://github.com/DonchoMinkov/castor/commit/f7a34d48533121ad6a40a75d1018975523d67616))
* **cmd:** take an episode's season and number as unsigned, not wrapped from negatives ([d1b97b1](https://github.com/DonchoMinkov/castor/commit/d1b97b1a5db9b62eb2d462f10c1edf92fee5a74d))
* **cmd:** use CLI framework for --debug flag instead of scanning os.Args ([bde9df8](https://github.com/DonchoMinkov/castor/commit/bde9df85371e264d23b8ce7d3578799ee388c7dc))
* **codec:** weigh a video encode above an audio one when picking a format ([e54c513](https://github.com/DonchoMinkov/castor/commit/e54c513e0b84b5be449857307916663e93bdeda3))
* config yaml should be optional ([#38](https://github.com/DonchoMinkov/castor/issues/38)) ([f8afcdd](https://github.com/DonchoMinkov/castor/commit/f8afcdd2f86396a155ff3f3df7d1854ba4edcc0c))
* **config:** keep defaults when a section is present but empty ([14f85b8](https://github.com/DonchoMinkov/castor/commit/14f85b8e5e120a943fe92f366d8065ec622e986e))
* **config:** reject unknown keys in owned sections ([e0bee3e](https://github.com/DonchoMinkov/castor/commit/e0bee3e50babb2de3a152eb31f3363e7f9f58421))
* **config:** report unreadable files ([a66b0f6](https://github.com/DonchoMinkov/castor/commit/a66b0f6ec5f499379a5e20a45faee8495f396950))
* correct HasVideo doc comment for lint ([327276a](https://github.com/DonchoMinkov/castor/commit/327276a2ce6880565f394da0630a10f20c4f5f6f))
* **dash:** bound timeline repeats by availability and period end ([f2e4073](https://github.com/DonchoMinkov/castor/commit/f2e4073eb74a3417c30aabdde9548dc655b58fac))
* **dash:** never give the last indexed segment a negative length ([b013156](https://github.com/DonchoMinkov/castor/commit/b01315690e272c6754141467b055c8273415a12a))
* **deps:** bump golang.org/x/mod v0.38.0 → v0.40.0 ([#62](https://github.com/DonchoMinkov/castor/issues/62)) ([1967fc7](https://github.com/DonchoMinkov/castor/commit/1967fc7514f67b74708103f43985381407c2543d))
* **deps:** bump golang.org/x/net to v0.60.0 ([afa8bfb](https://github.com/DonchoMinkov/castor/commit/afa8bfbe82d3680b5aef384ed395c38cf6888f18))
* **deps:** move to Go 1.27.3 and next 16.4.3 for known vulnerabilities ([d02e7b8](https://github.com/DonchoMinkov/castor/commit/d02e7b89e69128e6845d0cce5c68355bb8b25d32))
* **device:** derive each family's SelfFetch from its own selfFetches() ([6a4b14c](https://github.com/DonchoMinkov/castor/commit/6a4b14c50e41176a49671cbde83d302fba3f483e))
* **device:** echo what the device advertises and notice when it stops ([35a4ce2](https://github.com/DonchoMinkov/castor/commit/35a4ce2f92e5631752f7486182fcfbd112c78386))
* **device:** judge a renderer gone by how long it went unanswered, not how many polls failed ([23ab401](https://github.com/DonchoMinkov/castor/commit/23ab4011320c839159dfda912082fb3ab88e1004))
* **device:** preserve poll cancellation ([4978832](https://github.com/DonchoMinkov/castor/commit/49788323f7f8c30d420898da2e640c050fca4be0))
* **device:** retry DLNA SetAVTransportURI/Play through transient 705 Transport is locked ([ece219c](https://github.com/DonchoMinkov/castor/commit/ece219c3fe9bfa8c9045b2f92bf4d4cbb10cb0f6))
* **devices:** bound device connections by the network timeout ([9e2e7be](https://github.com/DonchoMinkov/castor/commit/9e2e7be156cc9683a28db80bdf4a5995e7dcb8d2))
* **device:** stop asserting a decode envelope for a device nobody identified ([6b15075](https://github.com/DonchoMinkov/castor/commit/6b1507588ccc39882b547168582c321ef6b58029))
* **dlna:** admit the sound an SCTE transport stream profile allows ([7ab20e3](https://github.com/DonchoMinkov/castor/commit/7ab20e31b1fdeb6a2560bfa006e7348e9aa20f31))
* **dlna:** bound pinned SSDP searches ([b210f80](https://github.com/DonchoMinkov/castor/commit/b210f80ac2826a90c9c707784675da747ba9bf77))
* **dlna:** cancel pending discovery ([dd414f8](https://github.com/DonchoMinkov/castor/commit/dd414f82aa855fed63e5daa8a8ac664c75262ee1))
* **dlna:** confirm playback after a timed-out Play request ([2f44f0a](https://github.com/DonchoMinkov/castor/commit/2f44f0a648019a82eca1e658b17cc71838250a97)), closes [#68](https://github.com/DonchoMinkov/castor/issues/68)
* **dlna:** deduplicate advertised playback capabilities ([f1e4869](https://github.com/DonchoMinkov/castor/commit/f1e4869c3f2ac4f67084d7b1852d300428aeb382))
* **dlna:** drive AVTransport and ConnectionManager v1, v2 and v3 ([#23](https://github.com/DonchoMinkov/castor/issues/23)) ([5e1d3d3](https://github.com/DonchoMinkov/castor/commit/5e1d3d34c520644b570dc0b6f59cbd7d16c8efac))
* **dlna:** drop Samsung's sec:CaptionInfoEx ([2358a20](https://github.com/DonchoMinkov/castor/commit/2358a20d403f43b00338f3850de236922ec227a7))
* **dlna:** give a container named without a profile the family default ([b65819a](https://github.com/DonchoMinkov/castor/commit/b65819a8db40191184cc5d617c92f9799b7df15d))
* **dlna:** ignore a stopped renderer's position and replace a paused stream ([d1f27ec](https://github.com/DonchoMinkov/castor/commit/d1f27ec9c0f38570622e065143cf0457ed78adfc))
* **dlna:** retain conservative playback when capabilities are unavailable ([ab4cdb8](https://github.com/DonchoMinkov/castor/commit/ab4cdb8cbf0e74fc99bb86ee8979933741c70761))
* **dlna:** search a typed address on SSDP's own port ([773fa61](https://github.com/DonchoMinkov/castor/commit/773fa61ee19f847f7bdf167235198830441052b8))
* **dlna:** stop pacing delivery to the renderer ([869f963](https://github.com/DonchoMinkov/castor/commit/869f963225d1390306332108dd879db17dae6aa5))
* docker image has old ffmpeg version ([b79e977](https://github.com/DonchoMinkov/castor/commit/b79e977f8932bd8f05ce573fd644292bc844833b))
* **docker:** cli cannot run in castor because of glibc version ([#40](https://github.com/DonchoMinkov/castor/issues/40)) ([52b2ad2](https://github.com/DonchoMinkov/castor/commit/52b2ad206864b4a715017503163affe3ca82f5cf))
* **docker:** hw capable ffmpeg with good flag support ([#43](https://github.com/DonchoMinkov/castor/issues/43)) ([70f4e4a](https://github.com/DonchoMinkov/castor/commit/70f4e4a145227c2df6005e7be794b122212e7181))
* **docker:** use host networking for LAN discovery and media delivery ([38ce22d](https://github.com/DonchoMinkov/castor/commit/38ce22d1760d69ad7dc0d08101fa1e9d9061ef1d))
* drop component prefix and use v in release tags ([7774782](https://github.com/DonchoMinkov/castor/commit/777478208d46aea2126bad3893b9bfeb0e882498))
* **encoding:** tone-map HDR once frames are shrunk ([6c1402b](https://github.com/DonchoMinkov/castor/commit/6c1402ba6b8679c7718d49e4f067f6517fd9d928))
* **execute:** keep every failure an attempt reports ([413d5cb](https://github.com/DonchoMinkov/castor/commit/413d5cb78c05ab384ba90142242882c7e2d8a35d))
* **extract:** bound each page and the snapshots taken of it ([22a764a](https://github.com/DonchoMinkov/castor/commit/22a764ade0667a623c531dbaadbedfa2b488293c))
* **extract:** reap headless Chrome on session teardown ([ab0edac](https://github.com/DonchoMinkov/castor/commit/ab0edace6e27a85d5fb4d0d34b302e6ecc5c8444))
* **ffmpeg:** count a kill as castor's only while ffmpeg is still running ([3c50a3e](https://github.com/DonchoMinkov/castor/commit/3c50a3e81ec4b0e59ddbd4e8eb0fb3636967f416))
* **ffmpeg:** detect HLS demux I/O errors as incomplete reads ([215964c](https://github.com/DonchoMinkov/castor/commit/215964c68c38c14540bc01e140ea6254d87d7cdd))
* **ffmpeg:** limit input protocols to the network ones a source is read over ([128a851](https://github.com/DonchoMinkov/castor/commit/128a8517957603c39a6a6463cc74f3c2fb5d5694))
* **ffmpeg:** pass -nostats to the puller invocation ([6377817](https://github.com/DonchoMinkov/castor/commit/6377817c77a3221d5092633613f069b731982c22))
* **ffmpeg:** reject subtitle burn-in without a video encoder ([f9e7772](https://github.com/DonchoMinkov/castor/commit/f9e77725e6c7febbc0d49861ad97c61e07fcca5a))
* **ffmpeg:** tell castor's own kill from a failure on Windows ([f211230](https://github.com/DonchoMinkov/castor/commit/f211230bbd40ecf2f7cd43cfcc0485047a70b58d))
* **follow:** answer a segment whose origin broke before its first byte with a bad gateway ([6a0be0d](https://github.com/DonchoMinkov/castor/commit/6a0be0dcfce3f289e1d90c843969630da8b73083))
* **follow:** let an empty first window leave the repackaging choice open ([cf59836](https://github.com/DonchoMinkov/castor/commit/cf598361a93925547b138d5905b8e2f869b97d4b))
* **follow:** read a timeline's first window again after a passing failure ([f0a7e37](https://github.com/DonchoMinkov/castor/commit/f0a7e3750201c10de5b5e4fa00ff9d8fbc50a876))
* **health:** describe stalled reads accurately ([424a8db](https://github.com/DonchoMinkov/castor/commit/424a8db6acd0a55cd470d2d6f1ecf106d07ea1ae))
* **hls:** accept short hexadecimal AES initialization vectors ([ef53b69](https://github.com/DonchoMinkov/castor/commit/ef53b6907cd3b4c3e5f512d07704db6259fef421))
* **hls:** honor receiver segment envelope capabilities ([c8b0ffc](https://github.com/DonchoMinkov/castor/commit/c8b0ffcf78851ff89a95138e2ba0d5ad48550f08))
* **hls:** open each segment on its own connection ([5425f90](https://github.com/DonchoMinkov/castor/commit/5425f90936276d04a8e9e30ea460a71c43eb3340))
* **hls:** read an init BYTERANGE without an offset from the first byte ([6ac3661](https://github.com/DonchoMinkov/castor/commit/6ac366179df50a0bac3291dd7b8be3dfa28c9875))
* **hls:** relay original fragments when no repackager is available ([5cf563f](https://github.com/DonchoMinkov/castor/commit/5cf563f36ad5e4c75d1bd9a5c5c56d964e02dd49))
* **hls:** release cancelled callers waiting for shared resources ([14e1e24](https://github.com/DonchoMinkov/castor/commit/14e1e24eb773127313cb388ac46bbcb128440a60))
* **hls:** restore direct playback for ordinary segments ([35f16f5](https://github.com/DonchoMinkov/castor/commit/35f16f5aa9851c42b50b184f403677f912cea73e))
* **hls:** retain settled renditions and reject protected companion audio ([867697b](https://github.com/DonchoMinkov/castor/commit/867697ba9c8aba8b899421939245fbc45c41783f))
* **hls:** send framed responses to ffmpeg readers ([bed33b3](https://github.com/DonchoMinkov/castor/commit/bed33b3daf198a7fcaeea4d7e042e431a6b4c408))
* let real request headers win over header-less captures ([01f47ee](https://github.com/DonchoMinkov/castor/commit/01f47ee42e540199be66ed658e0ddad8b927cf12))
* **log:** stop logging the healthy watch gate and ffmpeg's routine lines ([97dffd7](https://github.com/DonchoMinkov/castor/commit/97dffd741c519ca59ccc3bbe0368356d20672f68))
* **media:** enforce segment write deadlines and count delivered bytes ([a3497c3](https://github.com/DonchoMinkov/castor/commit/a3497c3ccd1edc4033b7e9c9fbeeb8e20bb8f53b))
* **media:** normalize BitDepths nil-vs-empty handling to match Profiles ([3f9ca62](https://github.com/DonchoMinkov/castor/commit/3f9ca6230445d7582595a0fb14ad0e07f0404d80))
* **media:** play audio-only streams without a video encoder ([b5c37f2](https://github.com/DonchoMinkov/castor/commit/b5c37f239c33b2d6e79bd202c46a9ee3df68c127))
* **media:** read HLS MIME aliases and report Stop as stopped ([#74](https://github.com/DonchoMinkov/castor/issues/74)) ([be6be9c](https://github.com/DonchoMinkov/castor/commit/be6be9ccf831a1dec2dd2b61bd026e6693bae1d2))
* **media:** respect advertised audio channel limits ([8792f34](https://github.com/DonchoMinkov/castor/commit/8792f34cac72d6252644f901301d17e42aeb317a))
* **mediaserver:** bound origin document reads and drain a stalled progress feed ([2c4467e](https://github.com/DonchoMinkov/castor/commit/2c4467e4f1dc8328572bdc87c24ec4b083e4cb75))
* **media:** support audio-only handoff and absent tracks ([b948415](https://github.com/DonchoMinkov/castor/commit/b94841563a4bf310e52f33ad3fb0d54849aeb61e))
* **media:** try another delivery when preferred encoding is unavailable ([d60919d](https://github.com/DonchoMinkov/castor/commit/d60919dbf280bac515d819f35c1db12869919738))
* pass ggml include path to cmake for Metal .m files ([7184338](https://github.com/DonchoMinkov/castor/commit/7184338958ecd9d2aee25d066fdb51ce9d72e06f))
* **probe:** read pixel component depth without confusing format layout ([d9322ed](https://github.com/DonchoMinkov/castor/commit/d9322ed1fdcedef533083508d2846c3b2c0fd5df))
* **probe:** weigh each audio track on its own bitrate ([b74ed3e](https://github.com/DonchoMinkov/castor/commit/b74ed3e2d883fd3d6da8b2f7a06c7be5d3d495d5))
* **rank:** admit a short stream as a last resort ([2ccd9f3](https://github.com/DonchoMinkov/castor/commit/2ccd9f3607caff231f3d4516035db63e92e91dd9))
* reconnect on HTTP 429 with backoff ([dc54a08](https://github.com/DonchoMinkov/castor/commit/dc54a082ae2fea9c39882cb20f828a2a65ae6410))
* **release:** clear quarantine through the install steps homebrew now expects ([#65](https://github.com/DonchoMinkov/castor/issues/65)) ([51448bd](https://github.com/DonchoMinkov/castor/commit/51448bd9cdea9a02928284f4b06dd656eef6ff32)), closes [#63](https://github.com/DonchoMinkov/castor/issues/63)
* **release:** restore postflight_steps in the brew cask ([#73](https://github.com/DonchoMinkov/castor/issues/73)) ([21d8840](https://github.com/DonchoMinkov/castor/commit/21d88404bc4f19114368a63e2b2d64f3dcf0aac9))
* remove non-canonical timestamp gate from LA-2 ([9242206](https://github.com/DonchoMinkov/castor/commit/9242206c7ab3c40eeed472f8b2a72a58c884d67a))
* remove v prefix from cask download URL ([f8b1855](https://github.com/DonchoMinkov/castor/commit/f8b1855626c5ad5a261857d3e3220e07f51a53ee))
* **replay:** keep credentialed stream paths distinct through recovery ([72331f6](https://github.com/DonchoMinkov/castor/commit/72331f61f74228feea8ff72f5201106e6d172853))
* **resolve:** never cast a variant that carries no video ([2c208c9](https://github.com/DonchoMinkov/castor/commit/2c208c97bdc6a53045c8c95f8dd89ec52f3eaeec))
* **resolve:** tiebreak equal-bandwidth candidates by height ([d2897d2](https://github.com/DonchoMinkov/castor/commit/d2897d2a02bdb0418b6efd6e8c4bc8aa7548346a))
* restore discover toggle and separate test environment ([ad54430](https://github.com/DonchoMinkov/castor/commit/ad5443056caf510f6286f379f5f5c9a8fd20d9e2))
* **roku:** refuse unsupported containers ([e5fada0](https://github.com/DonchoMinkov/castor/commit/e5fada07ce28433e19d5f0d3e004efc29236aaa3))
* **roku:** reject malformed app lists ([81f1cb7](https://github.com/DonchoMinkov/castor/commit/81f1cb775afc990a94cd72d8e6fd3681c9687645))
* **roku:** reserve discovery time for device names ([d603047](https://github.com/DonchoMinkov/castor/commit/d60304730cf314cd1112a77a87b8789bbb537128))
* **roku:** validate app lists and support IPv6 endpoints ([8a88261](https://github.com/DonchoMinkov/castor/commit/8a8826144bedf3c0951acae46f84e2914b8f7a35))
* **rpc:** validate requests and downstream responses at service edges ([0a3d24c](https://github.com/DonchoMinkov/castor/commit/0a3d24c2c1acd3a3509587c173c8fc006715f793))
* **scraping:** bound browser capture and preserve redirect credentials ([720dc35](https://github.com/DonchoMinkov/castor/commit/720dc35232018912ecdff6f3d05f79edbafa8e78))
* **scraping:** parse bounded manifest evidence and inherited DASH URLs ([e574aca](https://github.com/DonchoMinkov/castor/commit/e574aca7b5f53f33db927b727fdff47789db0e33))
* **scraping:** preserve resolver cancellation status codes ([0eb34e1](https://github.com/DonchoMinkov/castor/commit/0eb34e152cb6df7df461c0dbbe8917ae2b8c881e))
* **scraping:** use backward capture iteration for go fix ([c74ca6d](https://github.com/DonchoMinkov/castor/commit/c74ca6d3bcf9dc6583e94033ccdaaee4be156e0a))
* send browser request headers to puller so hotlinked streams work ([e8bec2f](https://github.com/DonchoMinkov/castor/commit/e8bec2ff92c14652a4add55dd611ce65afde235b))
* send browser request headers to puller so hotlinked streams work ([51b4102](https://github.com/DonchoMinkov/castor/commit/51b41022cc829821c532c6e75c5f0d1f2c98d142)), closes [#14](https://github.com/DonchoMinkov/castor/issues/14)
* **settings:** check required sections and name failures by config key ([386cf9b](https://github.com/DonchoMinkov/castor/commit/386cf9bf9019b1077c7f0f4aeefdb9c32e9abef8))
* **source:** follow re-signed segments once and bound what is buffered ([d435561](https://github.com/DonchoMinkov/castor/commit/d435561fde363dd7237fd71879a8242bfb63a75a))
* **source:** preserve cancellation during stream ranking ([59af7ce](https://github.com/DonchoMinkov/castor/commit/59af7ce4873aa5d45e3ece663d604dcae783d0b1))
* **source:** preserve unresolved playlist failures through completion ([0e54b30](https://github.com/DonchoMinkov/castor/commit/0e54b304a3286ffb1eeb23dddc6580a9ee64bb4c)), closes [#68](https://github.com/DonchoMinkov/castor/issues/68)
* **source:** report fallback from selected audio track ([90ca89c](https://github.com/DonchoMinkov/castor/commit/90ca89c72e91abe7fdd83ed49807539b32651754))
* **source:** retain declared codec levels for decoder limits ([251d08e](https://github.com/DonchoMinkov/castor/commit/251d08eaeb2d43c6e383c69f753c3785581c8444))
* **source:** validate media ranges and abort truncated segment responses ([fe46add](https://github.com/DonchoMinkov/castor/commit/fe46adde0bbc804c234d2f7aab9a3ab364be6a3e))
* stream buffers too much ([18663b7](https://github.com/DonchoMinkov/castor/commit/18663b7116dca0a88d892da3929d7d9ee2312236))
* **streaming:** follow production for open byte-zero live ranges ([1729928](https://github.com/DonchoMinkov/castor/commit/1729928a5fdba7e62d554bd122917ce8b6c2c233)), closes [#68](https://github.com/DonchoMinkov/castor/issues/68)
* **stream:** keep a paused device's connection open ([3c0a151](https://github.com/DonchoMinkov/castor/commit/3c0a1517f73b118e37aee72231cbb378c51460c4))
* **subtitles:** ask for a language in whisper's own codes ([c6845ef](https://github.com/DonchoMinkov/castor/commit/c6845ef8722bd6c5ceba35f3629f3c945f3f7e81))
* **subtitles:** ask Whisper for the two-letter code of a three-letter preference ([e6acc30](https://github.com/DonchoMinkov/castor/commit/e6acc308b28c70ff75b622525e70108ea0f868de))
* **subtitles:** select multilingual models and cancel transcription safely ([1b653b0](https://github.com/DonchoMinkov/castor/commit/1b653b00cf8bed70a519d64a2d4872ee3a6c162d))
* suppress unchecked Close() lint warnings ([52f06bd](https://github.com/DonchoMinkov/castor/commit/52f06bdc5de5d7cac86034e2abb655021aa55f1c))
* **timeline:** count a seam in the discontinuity sequence when its tag scrolls off ([03460d6](https://github.com/DonchoMinkov/castor/commit/03460d63e301bdbc133c0fe2ae91530a30668246))
* **timeline:** never republish a segment a lagging edge lists again, however long ago it was trimmed ([7872a24](https://github.com/DonchoMinkov/castor/commit/7872a240d4a6d6440fadedca7ce6a6a855224291))
* **tmdb:** honor proxy settings and dial timeouts ([4409be3](https://github.com/DonchoMinkov/castor/commit/4409be30e42529bcb45206ae0066f73ca059aa8a))
* **transcode:** declare a seamed program's discontinuity threshold once, before its inputs ([ce90404](https://github.com/DonchoMinkov/castor/commit/ce90404858db6532bf9547743884078689580c4d))
* **transport:** drain work after listener failures and release startup ports ([ab99005](https://github.com/DonchoMinkov/castor/commit/ab99005cc71498b3ab1c763c6ca25bdedba878d0))
* **transport:** keep bearer credentials on the configured origin ([416c150](https://github.com/DonchoMinkov/castor/commit/416c150fc2c289e87a4bcf19599542df9b48a589))
* **tui:** start no program on a done context ([7db26af](https://github.com/DonchoMinkov/castor/commit/7db26af07f8d1f0f4d8edcdbf57395ec6913ad4d))
* **whisper:** verify downloaded models against pinned SHA-256 ([2deb93e](https://github.com/DonchoMinkov/castor/commit/2deb93e87e5a03366cb76410fa8ee5327a306067))
* wire picked device name into config before browse ([1b4a204](https://github.com/DonchoMinkov/castor/commit/1b4a20482d5bf9d3c8a500e345016e221bfd0d14))


### Performance

* **media:** avoid cloning probe data ([f53452d](https://github.com/DonchoMinkov/castor/commit/f53452de852031982bec5d984083d7a62b955d6e))


### Refactors

* adopt newer standard library idioms ([4d6a130](https://github.com/DonchoMinkov/castor/commit/4d6a130f497f719f40380f7db51c80525361814e))
* **api:** build a session's watchers with it, not on the first subscribe ([d725bdb](https://github.com/DonchoMinkov/castor/commit/d725bdb542f4d8bc6105f6da0c71ecd3911debd4))
* **api:** build the server relay's proxy once, reading the route's values per request ([7fa7536](https://github.com/DonchoMinkov/castor/commit/7fa75363d8df29dffa367221cc2c10b20dad28ef))
* **api:** carry a stream's headers as one value each ([978e309](https://github.com/DonchoMinkov/castor/commit/978e309b0d8fd3e945ad2150aa8e91853350bedc))
* **api:** count in unsigned integers wherever nothing can be negative ([37c12ea](https://github.com/DonchoMinkov/castor/commit/37c12ea4c71f0060adc2910bf347d11e3a16baa3))
* **api:** drop rules and comments the contract already states otherwise ([99a82d6](https://github.com/DonchoMinkov/castor/commit/99a82d63e8bac56d35f689c35abea6ff26803f60))
* **api:** hold a cast's lifecycle in a looplab/fsm machine ([53d5033](https://github.com/DonchoMinkov/castor/commit/53d50339c68cab167798767e1f707a59295bf876))
* **api:** hold to the contract what a client sends, and say less in its comments ([b687454](https://github.com/DonchoMinkov/castor/commit/b6874543a1066683ba9940a908756bd23d600bb4))
* **api:** leave a watch's log level unset to ask for none ([cbfadb1](https://github.com/DonchoMinkov/castor/commit/cbfadb1c8ce861a3363fe6a044aeaee0d6202130))
* **api:** lend a cast one device, so its commands carry no handle ([ea1a25c](https://github.com/DonchoMinkov/castor/commit/ea1a25cf6297ea0051d81a89d291080600568102))
* **api:** lend a device with whether it fetches for itself, not a whole profile ([64aadf8](https://github.com/DonchoMinkov/castor/commit/64aadf8bd55d03b8866747dfd1c22ee95e966e84))
* **api:** name the cast RPCs Start and Stop, as every other RPC names its verb alone ([167c015](https://github.com/DonchoMinkov/castor/commit/167c01584c9e9ecbcbec371ccd8dd96fd84ecf92))
* **api:** name the device families after what they hold ([7a8fed1](https://github.com/DonchoMinkov/castor/commit/7a8fed176726f4dd6753fef0379336840394dc08))
* **api:** own remote sessions and join device observers ([8128d94](https://github.com/DonchoMinkov/castor/commit/8128d9430476077f4f7f3fd316383c7a2d267484))
* **api:** read a watch's end one way, and name every refusal the server makes ([0cf6c65](https://github.com/DonchoMinkov/castor/commit/0cf6c6529410b33a6e205e434c2bd6cb0d944249))
* **api:** reduce a cast's status to its counters ([4761605](https://github.com/DonchoMinkov/castor/commit/476160505333edee8da611bf64c290a99282b8b2))
* **api:** wait for a device for the undriven constant, not a field set to it everywhere ([340e689](https://github.com/DonchoMinkov/castor/commit/340e689805ca7456c2f6e397bc2b2a675d13bf5e))
* **app:** drop the unused casts slot ([27dee22](https://github.com/DonchoMinkov/castor/commit/27dee22232e9ff7314c542771718ce5252eb52e9))
* **app:** keep one cast submission path ([5c29ced](https://github.com/DonchoMinkov/castor/commit/5c29ced52f7ee817f2a70ddac72188c6f1818ee7))
* **app:** query casts directly ([f05cea1](https://github.com/DonchoMinkov/castor/commit/f05cea12cd9a6b5a9a333e35b3ba7f89f87ac5c4))
* **app:** use one API transport ([c769b9a](https://github.com/DonchoMinkov/castor/commit/c769b9a7fa92a92a6485eef46740306bc31063eb))
* **browse:** read fields directly instead of through one-line accessors ([8a99dc8](https://github.com/DonchoMinkov/castor/commit/8a99dc89a680b4412222fc04f8b699edd23e1243))
* **cast:** add SelfFetch renderer capability ([916e1c8](https://github.com/DonchoMinkov/castor/commit/916e1c83db151f8ca2e1b808a6b427b1326981b1))
* **cast:** capability-driven composition engine ([8001365](https://github.com/DonchoMinkov/castor/commit/800136546c38102dcadbd15a109f692908695437))
* **cast:** cast straight through attempt, and drop what only tests or nothing reached ([aedf957](https://github.com/DonchoMinkov/castor/commit/aedf9572fc65a0bc5539995cc6b6aa0fd723e182))
* **cast:** collapse deviceConnector and cueSource single-implementation interfaces ([63c2111](https://github.com/DonchoMinkov/castor/commit/63c21115fe8cd228f1117cc92eec8e46339a2e22))
* **cast:** coordinate typed preparation and readiness stages ([1c57a81](https://github.com/DonchoMinkov/castor/commit/1c57a815e0c037d7fbdc57fa69656e8098bd03aa))
* **cast:** declare one Listeners port, in deliver, and open every delivery through it ([0a4d1bc](https://github.com/DonchoMinkov/castor/commit/0a4d1bc80b29be0926df5c3f5fe6d9856c59f63c))
* **cast:** establish liveness once, and give the encoder one owner ([3bd32f0](https://github.com/DonchoMinkov/castor/commit/3bd32f082d1ad77c909a6d5061b85780320ca5e0))
* **cast:** finish renaming read plans to fetch plans and candidates to streams ([3c8739e](https://github.com/DonchoMinkov/castor/commit/3c8739e3617b9ecbb358d2dd0870f0fecd60e519))
* **cast:** fold single-file packages into their parents ([102610f](https://github.com/DonchoMinkov/castor/commit/102610f98bad92d95fbeb642a095c6c200c22e85))
* **cast:** leave a slow source to the device ([5e4f489](https://github.com/DonchoMinkov/castor/commit/5e4f489287a333fce0ff9547b4dfa94d9118a838))
* **cast:** let every table answer, and keep the spine a leaf ([1584e6d](https://github.com/DonchoMinkov/castor/commit/1584e6d20eca9a4bd12f2fa4feac32fb3ef2a007))
* **cast:** make stream pathologies data the cast layer can act on ([5839f94](https://github.com/DonchoMinkov/castor/commit/5839f94d87a7e616a96f2038a029bfbeec289769))
* **cast:** name read and watch by what they decide: fetch and health ([9b46f4c](https://github.com/DonchoMinkov/castor/commit/9b46f4c02bf48c923732a99d6d0d2ad16058ec04))
* **cast:** open deliveries through a Listeners port, under the cast's context ([5be3f42](https://github.com/DonchoMinkov/castor/commit/5be3f4237ced8976b40e63edc6c85c4178259f1a))
* **cast:** run an attempt on the values its steps return, and drop the indirection around it ([8d70075](https://github.com/DonchoMinkov/castor/commit/8d7007539e710c1dbe206efbf6f74f803d4d2193))
* **cast:** stand in a Turns nobody hears once, not a nil check at each turn ([bb167b2](https://github.com/DonchoMinkov/castor/commit/bb167b2af712662cbd047f4e4bd0d7625a5f0f19))
* **cast:** tier renderers below shared building blocks ([0357457](https://github.com/DonchoMinkov/castor/commit/0357457afee4f3e0ceb052658fcb0fdcd214e812))
* **client:** leave the contract's rules to the server, and say plainly when it refuses ([5d1d3f9](https://github.com/DonchoMinkov/castor/commit/5d1d3f9417a6d9b6379be0f9e201014dd898ba34))
* **client:** name the LAN address port Address, as one address it is ([9572fb3](https://github.com/DonchoMinkov/castor/commit/9572fb3bb4b084733153462290ecf1cca2b4eb60))
* **cli:** name and group the castor command line ([4ee4d51](https://github.com/DonchoMinkov/castor/commit/4ee4d513b8692c0bfedaa8d9de6f2e60bc611f44))
* **cmd:** build the missing TMDB key error with errors.New, having nothing to format ([0b01801](https://github.com/DonchoMinkov/castor/commit/0b01801a3f380abd32c5b59f0c7d909a1c25d914))
* **cmd:** load config with a method, and inline the forwarders around it ([af4f3af](https://github.com/DonchoMinkov/castor/commit/af4f3af9ce08999e18e548d51c5b6f14af9f6a2c))
* **config:** connect through remote.url and serve as castor server, one section each ([b3e3764](https://github.com/DonchoMinkov/castor/commit/b3e376469ee64d6ce9a5af4b69442ff10cf5b139))
* **config:** group service settings and reject unknown keys ([07bd158](https://github.com/DonchoMinkov/castor/commit/07bd15860fc660f0627c781e561be7c81d3758fc))
* **config:** identify a link with its cast's own resolver ([dd6f165](https://github.com/DonchoMinkov/castor/commit/dd6f165b7127f153b457632370942f87a80c59d8))
* **config:** iterate struct fields with reflect iterator ([066e2b6](https://github.com/DonchoMinkov/castor/commit/066e2b65881257f10b17d8af6b80ebd327326717))
* **deliver:** open deliveries on their Opening, with what is written where passed alongside ([b8ee3db](https://github.com/DonchoMinkov/castor/commit/b8ee3db6bc095121c207a9c9154eebe55efd4a74))
* **device:** carry a located device through whole ([3b5e172](https://github.com/DonchoMinkov/castor/commit/3b5e172db4fe87961c8e7c3ea1c649ac0e6c3d2c))
* **device:** dispatch renderer families through a strategy registry ([58d41f5](https://github.com/DonchoMinkov/castor/commit/58d41f598a9285e3b3be910468dc25d603d22728))
* **device:** drop what renderers and screens carried for nobody ([4dfd99b](https://github.com/DonchoMinkov/castor/commit/4dfd99b817d5625dcb74acef31367bceb0502783))
* **device:** hold constants every caller passed as parameters ([f87eb7a](https://github.com/DonchoMinkov/castor/commit/f87eb7acb92c0c110054f7a5fcf041b2285d5435))
* **device:** name a pinned device's endpoint in its family, not the lease ([8cd6c2f](https://github.com/DonchoMinkov/castor/commit/8cd6c2ff8231cc945c712126d1378850c0ef8ad0))
* **device:** separate discovery from device control ([7dbda84](https://github.com/DonchoMinkov/castor/commit/7dbda84db862d174c64bb94c98bd79f362b0338c))
* drop the probing and extraction layers that held nothing ([e9bf5c1](https://github.com/DonchoMinkov/castor/commit/e9bf5c1acc71789b4248a087695fa9fb704456d8))
* drop the standalone castor-api and castor-media binaries ([1955a32](https://github.com/DonchoMinkov/castor/commit/1955a321f79f8ced8ede5c6f5c525867c87c6f12))
* drop what media and subtitle carried for nobody ([bf2eca2](https://github.com/DonchoMinkov/castor/commit/bf2eca22948c9ebb6ac358e74774d384b46ea142))
* **e2e:** drop unused bookkeeping ([53496e6](https://github.com/DonchoMinkov/castor/commit/53496e6da47f0c2e7a278fe2585eb6a6471af12d))
* **execute:** call what an attempt keeps its files in a directory, not a one-field workspace ([f5451c3](https://github.com/DonchoMinkov/castor/commit/f5451c332b1427c1a74c363bb0f820942257e735))
* **extract:** drive the page and parallel extraction without single-use callbacks ([55b8b35](https://github.com/DonchoMinkov/castor/commit/55b8b35bc3c1fb9c1452c9f9aedc961299f0782a))
* **extract:** log what a page capture finds under the extraction's context ([630d197](https://github.com/DonchoMinkov/castor/commit/630d1975f53635ac7c8fac1c1e41c766330c0ff2))
* **ffmpeg:** centralize startup resource cleanup ([b32be3e](https://github.com/DonchoMinkov/castor/commit/b32be3e2d741e5eb43e2051303785bd06604010b))
* **ffmpeg:** use inherited pipes for Unix side outputs ([76e5798](https://github.com/DonchoMinkov/castor/commit/76e579854b9ea1d4123583be8acb650d663a8f3d))
* file each screen with what it picks: titles and devices ([d650c6c](https://github.com/DonchoMinkov/castor/commit/d650c6ca2fb250e76f6b99c3e73018ada17a29a5))
* give the API server and the media server the same shape ([04ac757](https://github.com/DonchoMinkov/castor/commit/04ac757f70998ba4d59bb8d3b7bcffbd97baf7b9))
* **hls:** centralize observed source compatibility ([868cf10](https://github.com/DonchoMinkov/castor/commit/868cf10a952275bbb1058a3a4116283a5e92848e))
* **hls:** separate AES decryption from fetching and bound key reads ([97aaa0d](https://github.com/DonchoMinkov/castor/commit/97aaa0df6e4db9b638332f41c88e32662215e51d))
* keep both servers' casts in one shared registry ([a11cb6d](https://github.com/DonchoMinkov/castor/commit/a11cb6d5a91c09bb1b81e53fe2b807a05f39315e))
* make the TUI and the process plumbing part of the binaries ([845dfb4](https://github.com/DonchoMinkov/castor/commit/845dfb4322101c9b6500b3f8cb7cdeaa2f8afae9))
* **media:** bind probe evidence and preserve explicit tracks ([7cb0645](https://github.com/DonchoMinkov/castor/commit/7cb064504e18ce82188d2df8504fa089e8719aa2))
* **media:** collect a program's header names in one place ([be04e5c](https://github.com/DonchoMinkov/castor/commit/be04e5c132e5a80aba928f9bef0d3e7359ee2aca))
* **media:** contain cast lifecycles and publication ownership ([cc96db5](https://github.com/DonchoMinkov/castor/commit/cc96db5b5d213830b1676affd0c8ae7e12a1d038))
* **media:** drop extraction leftovers ([8523f45](https://github.com/DonchoMinkov/castor/commit/8523f450cb00f0fa4c5c36b2786f28577f24a113))
* **media:** isolate segmented source decoding by format ([90fc7e3](https://github.com/DonchoMinkov/castor/commit/90fc7e33eaeb67a38fe57fdb966008ce30c23f14))
* **media:** name and group the ffmpeg, probe, media and subtitle tools ([41409bb](https://github.com/DonchoMinkov/castor/commit/41409bbfd76fd87e99f7fee38b19fb6ce666a634))
* **media:** name and group the source and extract packages ([03359d9](https://github.com/DonchoMinkov/castor/commit/03359d9778b2303f55b293833971407a5e2a37e9))
* **media:** name the cast runtime after what it does ([191eb87](https://github.com/DonchoMinkov/castor/commit/191eb877b6c0785b03b9d39dc7bac92ca6fd391f))
* **media:** simplify FormatForContentType to return (FormatInfo, bool) ([362ddc5](https://github.com/DonchoMinkov/castor/commit/362ddc5c734fa0bda072b5c38f0dc52ce1921d8b))
* mirror DLNA discovery on the chromecast pattern ([8123012](https://github.com/DonchoMinkov/castor/commit/812301212815791244c43a2aa6d5d92b74dbaa8c))
* modernize Discover and gate device interface impls ([2db6d91](https://github.com/DonchoMinkov/castor/commit/2db6d919bb349c1dfdaaec42bef1e537e9f0d834))
* **output:** answer segment requests through the opening ([6242595](https://github.com/DonchoMinkov/castor/commit/62425956da906ac5a3fbf5302b81d37771691b09))
* **probe:** inline input tolerances ([c5a376a](https://github.com/DonchoMinkov/castor/commit/c5a376a9d34b0a522195c20f31e892281392eed2))
* **proto:** name subtitle preference branch for its policy ([cb5f4f2](https://github.com/DonchoMinkov/castor/commit/cb5f4f22e477253986ca27852904990c907c1801))
* **proto:** remove compatibility reservations and compact fields ([828055a](https://github.com/DonchoMinkov/castor/commit/828055aca6e2aa200c2719866d4559cf7367d196))
* **proto:** state the contract's rules with protovalidate's built-in checks ([34c7765](https://github.com/DonchoMinkov/castor/commit/34c7765e779b0d8bcd7e32eaae8e34ec59fdd6c0))
* **proto:** type video support by codec ([49089d4](https://github.com/DonchoMinkov/castor/commit/49089d4cebcc82acbbe7c7fb0fca87b2ad8881d9))
* **release:** give brew its own job and run both channels after publish ([6c443a3](https://github.com/DonchoMinkov/castor/commit/6c443a3de870d9852fcb18b80b6ccaff75e7f4fe))
* remove subtitle font customization support ([43347c9](https://github.com/DonchoMinkov/castor/commit/43347c94c9eecd6a4461d389f860c5f34beb2f4c))
* **replay:** remove the now-unused token bucket ([5ff5fba](https://github.com/DonchoMinkov/castor/commit/5ff5fba4c28ccb30f84e14d487a58e906f108f85))
* **resolve:** decode HLS playlists with a spec parser ([c62c6e8](https://github.com/DonchoMinkov/castor/commit/c62c6e8e22f893492292d3d22dd12017583407ee))
* **resolve:** express resolution as the facts it establishes ([a0b3ce5](https://github.com/DonchoMinkov/castor/commit/a0b3ce5e9c424fa0259003c09b7ba6c92a5517f1))
* **rpc:** isolate playback contracts ([44a1667](https://github.com/DonchoMinkov/castor/commit/44a1667626f4570570f31b572ec9c6ecdad1613f))
* **rpc:** split audio and video codecs ([8c34300](https://github.com/DonchoMinkov/castor/commit/8c34300eaf0e2f8d28e1032404db24a8a0d8d39e))
* **rpc:** type device families ([956bcbc](https://github.com/DonchoMinkov/castor/commit/956bcbce904f677ae4ae7b3096a664576fa952b0))
* **rpc:** type stream metadata ([a792468](https://github.com/DonchoMinkov/castor/commit/a7924688e25f7edcea913018692e831836241ea2))
* run every state machine through one typed machine ([695ac81](https://github.com/DonchoMinkov/castor/commit/695ac8152e58248b69027b1fc2c1f85472fb1cc1))
* **scraping:** emit generated candidates and keep document inspection private ([42c4927](https://github.com/DonchoMinkov/castor/commit/42c49272dbf049c7c1aee97983fabe484ddd27d4))
* **screens:** move the browser, the picker and the logger to Charm v2 ([46318b4](https://github.com/DonchoMinkov/castor/commit/46318b4fef4a012ade429e10ac8fcca476f2285c))
* **screens:** name the bar colours, draw every list with one delegate, ask the background once ([4eb0108](https://github.com/DonchoMinkov/castor/commit/4eb0108930bdd8446ca299bd40d177a400dcf238))
* **settings:** spell proto enums in configuration by their contract names ([50814f2](https://github.com/DonchoMinkov/castor/commit/50814f2b08f46c4598190245a72ad17a289c10fd))
* **source:** call a found link a Stream, as everything that hands it on does ([20b6364](https://github.com/DonchoMinkov/castor/commit/20b636486f5acf23b654b9c7cf593f436ec8102d))
* **source:** deduplicate MIME tables and unexport Extractor.Extract ([50c1886](https://github.com/DonchoMinkov/castor/commit/50c1886e601b4e9208ae7671ac3261484529a332))
* **source:** give each port only what its implementations use ([c053363](https://github.com/DonchoMinkov/castor/commit/c053363bb3ae3c5fd7311baf4c464f3f45d0fef1))
* **source:** identify a link without a header nobody passes, and inline config's one-line helpers ([768d468](https://github.com/DonchoMinkov/castor/commit/768d468e53d6dda610d7298fb1c8b4dea0e01666))
* split castor into sealed media server, API server and TUI tiers ([4fa3c3f](https://github.com/DonchoMinkov/castor/commit/4fa3c3f674a3d7ae484213f660a0af17fbd58eb0))
* split HLS fetch from parse ([c84436e](https://github.com/DonchoMinkov/castor/commit/c84436e35c6ea11fa5e9c2ccb0a074f7ec40cbc1))
* split the cast into policy, engine and execution, and give sources and devices one strategy each ([8d25172](https://github.com/DonchoMinkov/castor/commit/8d25172708554d76919b6dd06b44f6d710c50f98))
* start both servers through transport.Listen and transport.Loopback ([b53ed87](https://github.com/DonchoMinkov/castor/commit/b53ed87ef36a310824c748740be9c8fc6c81330c))
* **subtitle:** name subtitle.Word and ensure the VAD model directly ([c32bfa0](https://github.com/DonchoMinkov/castor/commit/c32bfa0c7e3170bb94f84294a5731d4da38b173b))
* **subtitles:** encode transcription within enabled selection ([fe4e1a4](https://github.com/DonchoMinkov/castor/commit/fe4e1a44d435b0920c7892e5d232f8c6e24c05e6))
* **test:** simplify recovery doubles ([08d39e7](https://github.com/DonchoMinkov/castor/commit/08d39e712ad712cb8dbf912260bebb41140952b5))
* **tmdb:** read release dates directly ([c4a0cf9](https://github.com/DonchoMinkov/castor/commit/c4a0cf9d2a7697059bfaa93fb493d53d772fa2e3))
* **tmdb:** remove dead Page.HasMore method and SearchResult.GenreIDs field ([ab17b0c](https://github.com/DonchoMinkov/castor/commit/ab17b0c33230f2da492aabd7576ad6f983c7258d))
* **transcode:** use output tuning directly ([9ecb4d3](https://github.com/DonchoMinkov/castor/commit/9ecb4d34c676ade00d8e2ce0cff129cec8791ee4))
* **transport:** split serving and the token rule out of transport.go ([0ac58b4](https://github.com/DonchoMinkov/castor/commit/0ac58b4bbe790be3dbf1e8ca3d14e7c2cabb55ff))
* type sentinel strings as named constants and enums ([145ba68](https://github.com/DonchoMinkov/castor/commit/145ba68d0967ace7e0fe41563b12b9848d2df52e))
* unexport what no other package reads ([58832a1](https://github.com/DonchoMinkov/castor/commit/58832a1b7437ae13f5963501933748e6d8c4d7c3))
* use explicit 2xx range check instead of the /100 trick ([d81308a](https://github.com/DonchoMinkov/castor/commit/d81308a8bea6ed6f6613083c634c41f4e6e8cc74))
* **whisper:** collapse WordSink interface and unexport EnsureModel/EnsureVADModel ([1c76a76](https://github.com/DonchoMinkov/castor/commit/1c76a7665715e07209ec7ec4c4038d0f2b567609))


### Documentation

* add Trendshift badge ([f848dbf](https://github.com/DonchoMinkov/castor/commit/f848dbf65d617c52525f25ac97b14062214dcc05))
* **architecture:** update the architecture documentation ([cb041a2](https://github.com/DonchoMinkov/castor/commit/cb041a221a632b29ed0b1145cb72209fe374d4f6))
* **browse:** remove stale comment on inspector.load ([faaa253](https://github.com/DonchoMinkov/castor/commit/faaa253cf7a6690721e15b7d543b552370d3e35a))
* condense architecture and show cooperating state machines ([9ca61c3](https://github.com/DonchoMinkov/castor/commit/9ca61c3b9eab7dfc3257f73d0197b74322fef017))
* **config:** say subtitle burn-in reaches DLNA only ([9a7c614](https://github.com/DonchoMinkov/castor/commit/9a7c614cd0d96b43691c40fb6bea92b34d4c0dd0))
* **container:** say what the package describes ([a113cf6](https://github.com/DonchoMinkov/castor/commit/a113cf6a4b2cd985eb7e1a7f818c2d844695eebd))
* **contributing:** hold the tree to feature slices in review ([392b04b](https://github.com/DonchoMinkov/castor/commit/392b04b300891c3d96352475b7fb91a7b0125de6))
* **contributing:** require Go 1.27.1 and set out what castor will not take ([265a322](https://github.com/DonchoMinkov/castor/commit/265a3229b8ffa64e4eb82c76c3c33ae5981f1992))
* describe lifecycle ownership and shared media publications ([6f9853c](https://github.com/DonchoMinkov/castor/commit/6f9853c5b56d60ed10a92cab5879d17709a567ec))
* describe observed HLS handoff boundary ([ef7aa21](https://github.com/DonchoMinkov/castor/commit/ef7aa216da5b907a80ac94f4e9dbf8687c4d3801))
* document how to verify the image SBOM and provenance ([3b237cc](https://github.com/DonchoMinkov/castor/commit/3b237ccc6e7e33a363ca68f642900b044ba4e553))
* document pinning a device by host ([51a8a9d](https://github.com/DonchoMinkov/castor/commit/51a8a9d6d8598aae86356d6809abd8dcf7151d00))
* document resolver max_height option ([435c0f0](https://github.com/DonchoMinkov/castor/commit/435c0f0eb3069a4e5375c64f58b516ce6bf3e9fb))
* drop stale references to the send pacer ([6301ebf](https://github.com/DonchoMinkov/castor/commit/6301ebfb4691d2689fae07c3c65cad3afadd2983))
* explain format owned segmented source reading ([49e5b0a](https://github.com/DonchoMinkov/castor/commit/49e5b0a74c122c715ddbdaf421eadc69aeaf6fb8))
* explain how castor works inside in ARCHITECTURE.md ([dce0e54](https://github.com/DonchoMinkov/castor/commit/dce0e54368bf6b393e2e14319ad74b0bbe8c96aa))
* give telemetry its own section in CONTRIBUTING ([2a46ff8](https://github.com/DonchoMinkov/castor/commit/2a46ff8018ffba919605f3c122329df96e720ba2))
* **media:** correct ProbeInfo's blanket unknown-value doc ([bce923d](https://github.com/DonchoMinkov/castor/commit/bce923df4e819826d6cdcb245dc6cbdaa036f20e))
* prepare Castor 2.0 migration ([#69](https://github.com/DonchoMinkov/castor/issues/69)) ([adea81d](https://github.com/DonchoMinkov/castor/commit/adea81d1bd021988fc4c087121fc87a4b9fd8e83))
* **readme:** add a table of the platforms castor runs on ([081772e](https://github.com/DonchoMinkov/castor/commit/081772e12ba42307604defd5d905a98c4c092d55))
* **readme:** add an npm version badge ([c7ebe67](https://github.com/DonchoMinkov/castor/commit/c7ebe674a03229e566d99fb97ee9ad8e0fd08a88))
* **readme:** add Installation section (Homebrew, Docker, source) ([7ba4e01](https://github.com/DonchoMinkov/castor/commit/7ba4e01d6de0721bac31a43c576c9e7adfdd10eb))
* **readme:** cover using castor, and leave its mechanics to ARCHITECTURE.md ([d16829d](https://github.com/DonchoMinkov/castor/commit/d16829dbfec14a12348993b04c151ffa3d7fa429))
* **readme:** fix stale commands, add config quickstart and screenshots ([fc80f3e](https://github.com/DonchoMinkov/castor/commit/fc80f3e307388868acc54cb080f626ed75a13206))
* **readme:** lead the quick start with brew, npm and a source build ([de5b244](https://github.com/DonchoMinkov/castor/commit/de5b2441d68111b0c14df63a7ddbaf3096be6f8b))
* **readme:** list community projects, starting with castor-android ([3d44b48](https://github.com/DonchoMinkov/castor/commit/3d44b480feda04c78507c3c12a5fa61210545e76))
* **readme:** redraw the mascot as a gopher in a beaver costume ([4297d83](https://github.com/DonchoMinkov/castor/commit/4297d83d1d0f17841ddbc62f94f081188a58a578))
* **readme:** rewrite as a short onboarding page ([9b05b73](https://github.com/DonchoMinkov/castor/commit/9b05b73901734a955128032a939e5b53c491d455))
* restructure installation, configuration, and docker sections ([54b6fea](https://github.com/DonchoMinkov/castor/commit/54b6fea44770f456ad33e25a7d699962fbe795ec))
* rewrite ARCHITECTURE.md around tiers, topologies and boundaries ([b51a765](https://github.com/DonchoMinkov/castor/commit/b51a76598af7db1ab2702938780d3d20b05c4172))
* say what the media server model does where comments and SECURITY.md still told the relay's ([d56fbba](https://github.com/DonchoMinkov/castor/commit/d56fbba81ac85894be7d2c843e33ed1396f0bfec))
* **security:** report vulnerabilities privately and warn about open servers ([702685b](https://github.com/DonchoMinkov/castor/commit/702685b18655e4c2e7f0fcd2e41c1fbbdfa6e41e))
* **security:** say castor serves plain HTTP and to terminate TLS in a proxy ([2b794d3](https://github.com/DonchoMinkov/castor/commit/2b794d3a21441040de51478c134a36ac37ebf12e))
* streamline setup and usage in README ([392fb47](https://github.com/DonchoMinkov/castor/commit/392fb47801b57ee02250d294349cd6633eba98b7))
* **telemetry:** add a provisioned Grafana dashboard and the local collector recipe ([2d62cf0](https://github.com/DonchoMinkov/castor/commit/2d62cf0c9d516347a8b03114c8025ca26ef7e7db))
* tighten the readme, contributing and security guides ([999efd3](https://github.com/DonchoMinkov/castor/commit/999efd3cbe39d159babc9b1a78b96a135081bc71))
* **transcode:** say the splice timestamp threshold holds for every input ([866fc2d](https://github.com/DonchoMinkov/castor/commit/866fc2d48316c2f591b5badba0d36f88f1ff3a8e))
* trim the service guides ([0b94163](https://github.com/DonchoMinkov/castor/commit/0b941638498be0ad5c64b9ccb06dc62b254941a8))


### Build System

* **app:** drop unused headless UI ([5fdf6f1](https://github.com/DonchoMinkov/castor/commit/5fdf6f1de086ef37b346a28e71c04164e03a8ee2))
* **app:** validate the web app in CI and wire the Tilt environment ([f5cc718](https://github.com/DonchoMinkov/castor/commit/f5cc718f76ddf2ec5cdb1051ab500d7cf398b96b))
* **deps:** bump Go to 1.27.1 and the direct dependencies ([cb17e1b](https://github.com/DonchoMinkov/castor/commit/cb17e1b003057cb9483dae80fce8b90529814248))
* **deps:** bump mp4ff, koanf and teatest, and keep node_modules out of ./... ([6c1fcf6](https://github.com/DonchoMinkov/castor/commit/6c1fcf66dbc0721aed6df44de38f9cf4b25c39c5))
* **deps:** bump whisper.cpp to v1.9.4 ([36a53a6](https://github.com/DonchoMinkov/castor/commit/36a53a6e63970f69e44ab507e24d635e577b70df))
* **docker:** attach an SPDX SBOM and SLSA provenance to the image ([5f8a135](https://github.com/DonchoMinkov/castor/commit/5f8a135144e82b0d97e9bfc5cdfcce87d8be1c93))
* **docker:** build image with docker bake ([7d004f0](https://github.com/DonchoMinkov/castor/commit/7d004f00c78f4372b88c1da2dc11bec76dec37f5))
* **docker:** limit the build context ([b9c2e7b](https://github.com/DonchoMinkov/castor/commit/b9c2e7b3638b821bef1e693b669dbf3b4cd54b03))
* drop the tooling that did nothing ([f529b96](https://github.com/DonchoMinkov/castor/commit/f529b9687e0add1f72de843db023c22950c3c543))
* move to Go 1.27 and the latest dependencies ([b20360d](https://github.com/DonchoMinkov/castor/commit/b20360d704200f200169582092451aacea5e26d6))
* **proto:** drop compatibility checks ([15350ac](https://github.com/DonchoMinkov/castor/commit/15350acb0d7e77f15b66b8c5576e6a80e704b336))
* **release:** rename the cask script to brew.sh ([95655df](https://github.com/DonchoMinkov/castor/commit/95655df3bdba8e37d4b947bc8e586aa958b0e2e6))


### Continuous Integration

* automate releases with release-please and on-demand canary previews ([#26](https://github.com/DonchoMinkov/castor/issues/26)) ([2ed9150](https://github.com/DonchoMinkov/castor/commit/2ed9150deb1bd8579092dfaf438f9a21da4a3c3b))
* bump download-artifact, setup-node and upload-artifact ([f47a1c6](https://github.com/DonchoMinkov/castor/commit/f47a1c6dd5fd3634779ca34e24c4bff5ebf08e6b))
* bump the action pins and lint tools, and gate on go fix ([5653757](https://github.com/DonchoMinkov/castor/commit/56537572a464954aca4867f01400c61ec5755dde))
* check only first-party packages ([26ffbe1](https://github.com/DonchoMinkov/castor/commit/26ffbe1d9a166f8858ab9d7abff9ecfa6a3059d7))
* drop v prefix from release tags ([51444bb](https://github.com/DonchoMinkov/castor/commit/51444bbb85870ffb041671db97500ac10798130e))
* fix empty release version and release on ci commits ([5a3b465](https://github.com/DonchoMinkov/castor/commit/5a3b465bdc1679bad45deaf400a1ede8f5b5d383))
* install ffmpeg 7.1 and keep go's download noise out of the deadcode gate ([aa6f273](https://github.com/DonchoMinkov/castor/commit/aa6f2735c94c7b3998e41250ea852e3bc8038efc))
* leave the e2e suite out of the test job ([aa940ce](https://github.com/DonchoMinkov/castor/commit/aa940ce1357d097976edc680a30fd52348fa160f))
* lint the contract, refuse breaking changes to it, and check gen/ is current ([b650802](https://github.com/DonchoMinkov/castor/commit/b6508027829306e3eb97ec34933d93555bf95507))
* lint the sealed tiers, keep castor-api cgo-free, and release the three binaries ([2f5c5bc](https://github.com/DonchoMinkov/castor/commit/2f5c5bc81c6b6da6cfc6ecda4a10f1333a91056a))
* **release:** publish only the castor binary ([329d3fb](https://github.com/DonchoMinkov/castor/commit/329d3fbcd0e5041c65de71a3367aebc1bc4c7b51))
* run go fix -diff as the gate itself, so a failure shows its diff ([55f356e](https://github.com/DonchoMinkov/castor/commit/55f356e9243ea5209078002ff89d4e9effc39df1))
* run once per PR, with -race, and a valid cask stanza ([3c5db61](https://github.com/DonchoMinkov/castor/commit/3c5db613e8cfdc13ded53a5097052ca633fbb8e5))
* scan Go and app dependencies for vulnerabilities ([9c606e7](https://github.com/DonchoMinkov/castor/commit/9c606e78e44a4332eb806472d206a4ac2fb620ed))
* skip push CI on main ([9e0c9f0](https://github.com/DonchoMinkov/castor/commit/9e0c9f0fedc9806f3272bfedb61dfc51d99765df))

## [2.5.0](https://github.com/stupside/castor/compare/v2.4.0...v2.5.0) (2026-10-27)


### Features

* **cast:** let the interactive cast run without a configured device ([61c8490](https://github.com/stupside/castor/commit/61c8490ec06070a82c0bb7687f093974683eec0b))
* **settings:** read the user's config directory, then the working directory's ([a726b44](https://github.com/stupside/castor/commit/a726b444e5631e43efb7be202edd10b8130e3f18))


### Bug Fixes

* **deps:** move to Go 1.27.3 and next 16.4.3 for known vulnerabilities ([f16ef1f](https://github.com/stupside/castor/commit/f16ef1f910e1f0cb2f600b81bcb9c9c6648f0ace))
* **settings:** check required sections and name failures by config key ([71a077c](https://github.com/stupside/castor/commit/71a077c192f9fbf4d74686df666649015054d0f0))


### Documentation

* **architecture:** update the architecture documentation ([15d0616](https://github.com/stupside/castor/commit/15d0616aca5f731728f60f39bc6856056d2efcba))
* **contributing:** require Go 1.27.1 and set out what castor will not take ([54d4398](https://github.com/stupside/castor/commit/54d4398e2ac622ff2caeb33c1953af33c861c5b2))
* give telemetry its own section in CONTRIBUTING ([ea35704](https://github.com/stupside/castor/commit/ea35704eadedd5210779a1b608c47edf25d375f6))
* **readme:** add a table of the platforms castor runs on ([2410b80](https://github.com/stupside/castor/commit/2410b802c227eafa1d19593c97316d4b48e8e40a))
* **readme:** list community projects, starting with castor-android ([435ea38](https://github.com/stupside/castor/commit/435ea38fd27a1067dcbbd8c481d274bb4c2a60e2))
* **readme:** rewrite as a short onboarding page ([02ef689](https://github.com/stupside/castor/commit/02ef6895fb72ba69a9dee9266a455ee5d64de0b9))
* **security:** report vulnerabilities privately and warn about open servers ([61e4908](https://github.com/stupside/castor/commit/61e49088441edf46cce704e4d73a94453b80124a))


### Continuous Integration

* scan Go and app dependencies for vulnerabilities ([87307d4](https://github.com/stupside/castor/commit/87307d4288f5986b18030ee7032cd9c008ac88a1))

## [2.4.0](https://github.com/stupside/castor/compare/v2.3.0...v2.4.0) (2026-10-26)


### Features

* **cast:** begin a cast at a position ([c3fde9f](https://github.com/stupside/castor/commit/c3fde9f41ab9d87495388ab7ff438ccc1ef75d09))
* **cast:** follow the device's link while it plays ([c7c3af8](https://github.com/stupside/castor/commit/c7c3af827c029adc7aa67efd7e0eba2c5a91c5ce))
* **cast:** go back to a better ranked link once the cast plays well ([0162f91](https://github.com/stupside/castor/commit/0162f9186e8bc7504e46d07877e542cfeb6602fc))
* **cast:** let the device play out what it took before stopping ([d0caa8d](https://github.com/stupside/castor/commit/d0caa8d335469ebd7292013656fa51d60527a495))
* **device:** report the device's position and its viewer's pause ([0408dd5](https://github.com/stupside/castor/commit/0408dd5efe72c977d6f60fde01618cf3e14f6d58))
* **dlna:** seek within the stream castor serves ([cc89147](https://github.com/stupside/castor/commit/cc891475be59151d7c71e9a9fbdc34a73c6d7b30))
* **rank:** rank links by the language of their sound first ([b833922](https://github.com/stupside/castor/commit/b8339222c015668b5c79f1e686f0d0d175b5a757))


### Bug Fixes

* **cast:** count what the encoders made where they read the buffer ([30bc249](https://github.com/stupside/castor/commit/30bc249c225cede7f52079dc0b2a7bc2fe41acd7))
* **dlna:** drop Samsung's sec:CaptionInfoEx ([3e8b521](https://github.com/stupside/castor/commit/3e8b521b5847a9ccff3416a88472edfb9e651f32))
* **execute:** keep every failure an attempt reports ([8f7f9ee](https://github.com/stupside/castor/commit/8f7f9eedd505e793dc5fc51ce2ac753cb61b8f85))
* **probe:** weigh each audio track on its own bitrate ([fd3a603](https://github.com/stupside/castor/commit/fd3a60372894bbb9cd3caa4bd606939c44019c13))
* **stream:** keep a paused device's connection open ([931677f](https://github.com/stupside/castor/commit/931677f34010b4ef09542bad939159b5fd77ffb7))


### Refactors

* **device:** carry a located device through whole ([2adc65e](https://github.com/stupside/castor/commit/2adc65ed34b17e2876a25f5232351fc3012c6be7))
* **output:** answer segment requests through the opening ([5af01c1](https://github.com/stupside/castor/commit/5af01c1b0d3adae3074a4b35be8bad2975f74ff3))
* run every state machine through one typed machine ([047076b](https://github.com/stupside/castor/commit/047076b4647e5f3814eddc3068bd923940fa7cd9))

## [2.3.0](https://github.com/stupside/castor/compare/v2.2.0...v2.3.0) (2026-10-22)


### Features

* **release:** give the npm launcher search keywords ([#77](https://github.com/stupside/castor/issues/77)) ([c0dc517](https://github.com/stupside/castor/commit/c0dc5177ff023cb60ddae90e73635dfcfd6aea18))


### Documentation

* **readme:** add an npm version badge ([1711a67](https://github.com/stupside/castor/commit/1711a67ce42008951d6e8b6224055809d66e4312))

## [2.2.0](https://github.com/stupside/castor/compare/v2.1.0...v2.2.0) (2026-10-22)


### Features

* **release:** ship the project docs in every npm package ([34ff4d9](https://github.com/stupside/castor/commit/34ff4d9f1e250fdbf8985d9bc2b0cb719fb0039b))


### Bug Fixes

* **media:** read HLS MIME aliases and report Stop as stopped ([#74](https://github.com/stupside/castor/issues/74)) ([56ac869](https://github.com/stupside/castor/commit/56ac86927476f22ae8321fa285e8bc3dcf9f4313))

## [2.1.0](https://github.com/stupside/castor/compare/v2.0.0...v2.1.0) (2026-10-22)


### Features

* **release:** publish the cli to npm through trusted publishing ([aa2510c](https://github.com/stupside/castor/commit/aa2510cbe60d1e67e25ee82fcf7003b7401e829e))
* **telemetry:** namespace OTel names and make logs say why ([e993388](https://github.com/stupside/castor/commit/e99338836b278be2e5708265e8ebd35d1f753605))
* **telemetry:** record state machines as one span per state ([7aaf50b](https://github.com/stupside/castor/commit/7aaf50beefbdda90a746a154eac86fd9e5c924e3))
* **telemetry:** second-scale duration buckets, semconv 1.43 and service version ([217f29d](https://github.com/stupside/castor/commit/217f29d4d6674dd5de7aefbc81a50a1812c6768c))


### Bug Fixes

* **codec:** weigh a video encode above an audio one when picking a format ([d466da9](https://github.com/stupside/castor/commit/d466da905b02e161b51f726d0d8f28d1cee9985a))
* **release:** restore postflight_steps in the brew cask ([#73](https://github.com/stupside/castor/issues/73)) ([3d022c0](https://github.com/stupside/castor/commit/3d022c03a62ffa732d60de498c4718a11bfcb3e9))


### Refactors

* **release:** give brew its own job and run both channels after publish ([0b8d943](https://github.com/stupside/castor/commit/0b8d943d4c62a768e26299561dcd74c2df07ddbb))


### Documentation

* **readme:** lead the quick start with brew, npm and a source build ([7869786](https://github.com/stupside/castor/commit/7869786ce73e3b66e2b2425c9a0bee7bc14796d6))
* **telemetry:** add a provisioned Grafana dashboard and the local collector recipe ([0a24a99](https://github.com/stupside/castor/commit/0a24a99b221ea9fb29c4a64ef0ab307ea5a9fcc4))

## [2.0.0](https://github.com/stupside/castor/compare/v1.9.0...v2.0.0) (2026-10-21)


### ⚠ BREAKING CHANGES

* Castor 1.x configuration must be migrated to the cast and servers sections. See the [1.x → 2.0 migration guide](https://github.com/stupside/castor/blob/main/migrations/1.x-to-2.0.md).

### Features

* **api:** drive a castor server for the renderers on the client's network ([b4f6349](https://github.com/stupside/castor/commit/b4f6349906fdc99fc7d471229726a998062fd9a0))
* **api:** hold every message to the contract both ways, with protovalidate and CEL rules ([0f2a520](https://github.com/stupside/castor/commit/0f2a5203e24ec629f528593e4182f7d1cb6807f4))
* **api:** log the address of the device a client lends, which the contract sends for that ([4205f3e](https://github.com/stupside/castor/commit/4205f3ee2c20d0838bcb6d2638a673ce91d09537))
* **api:** make the server the media server, which TVs fetch from and which outlives its client ([f9aabf6](https://github.com/stupside/castor/commit/f9aabf6e4524555fb7bba06c9574fce0f18b95df))
* **api:** serve casts behind the contract, driving renderers only through a client ([e48dd4b](https://github.com/stupside/castor/commit/e48dd4b75b2752f53422495bbec1edb2e8525384))
* **api:** state the cast contract in protobuf, generated with buf for Connect ([3d3bf60](https://github.com/stupside/castor/commit/3d3bf60dfe5d706edcfd6a135d4ac6e73bc95e78))
* **app:** add the web client ([e295db7](https://github.com/stupside/castor/commit/e295db7772fc0904dbcc643f3941617dd503a57c))
* **app:** expose manual targets and per-cast playback options ([5f91b27](https://github.com/stupside/castor/commit/5f91b279c8b525d481aee8a5f786cd8e6e57a716))
* **cast:** negotiate subtitle delivery and own backend lifecycles ([9b5714c](https://github.com/stupside/castor/commit/9b5714c39a0994c6a16401cd9203aaba93ef2ecf))
* **cast:** pass a source's HLS captions to the device and play the audio language asked ([893c449](https://github.com/stupside/castor/commit/893c4496f22252c6b3bbbc7310e4323b82dab518))
* **cast:** resolve a device by id and refuse an ambiguous name ([13f6abb](https://github.com/stupside/castor/commit/13f6abb0bdf3031647922628b85914fc39bc92f3))
* **cast:** start a device once the read holds thirty seconds ([7966a51](https://github.com/stupside/castor/commit/7966a516af63b8cf13ffc12e1809a563ff431814))
* **cast:** tell a Turns port each attempt and revision a cast takes ([08de916](https://github.com/stupside/castor/commit/08de916e26457a4f8f219f330fdde1ac8022b452))
* **cli:** also write log lines to castor.log in the user cache directory ([e29bb19](https://github.com/stupside/castor/commit/e29bb19d8e103d38cfafb5c1b148de2835f155bc))
* **cli:** compose the scraping service ([20dda9d](https://github.com/stupside/castor/commit/20dda9db2101ed7580233e95d713c1cc0b474d91))
* **cli:** split castor api-server from castor media-server ([8e70bc8](https://github.com/stupside/castor/commit/8e70bc86a7f7737c51797fce5d02e618974c78fa))
* **cmd:** cast through the API, served in process or by castor api server ([6eec870](https://github.com/stupside/castor/commit/6eec8706629896389b67b2905184e0c533a1aedd))
* **cmd:** hold the client's log lines back while a screen is up, and write them after ([e0a7035](https://github.com/stupside/castor/commit/e0a7035decc611e870fbd0696e58a4d7973a6734))
* **cmd:** show a cast's warnings without --debug, and the embedded engine's own lines with it ([f8459af](https://github.com/stupside/castor/commit/f8459af3499b62c06019aa7f837034e8ab2735f2))
* **config:** allow custom FFmpeg tool paths ([6c3893a](https://github.com/stupside/castor/commit/6c3893a697eccf0c09c3bfb1a7a7bb38be7bebeb))
* **config:** refuse a subtitle language that is neither a BCP-47 tag nor auto ([a7aa3c2](https://github.com/stupside/castor/commit/a7aa3c2c42a5571ac45e5d590b504ecb93e89ca6))
* **device:** pause and resume the lent device ([a6424cd](https://github.com/stupside/castor/commit/a6424cd503732353fe147ea7b38e6981b9089d77))
* **docker:** run media-server and api-server as separate compose services ([2f6570d](https://github.com/stupside/castor/commit/2f6570d33ad838c141e62767a4e449ae3231e1c5))
* **docker:** run the scraping service ([acc5583](https://github.com/stupside/castor/commit/acc55839663a32265be9d68b2b4d22a971742661))
* **ffmpeg:** use private named pipes for Windows side outputs ([17f19cb](https://github.com/stupside/castor/commit/17f19cb70af5f76b7238be2359bab778fe412df6))
* **health:** hold a device its read falls behind instead of letting it run dry ([8e773d0](https://github.com/stupside/castor/commit/8e773d07aa31a771f3b54c2a5dd1ad5e4f51d69c))
* **health:** start a cast on a short cushion and judge it by its whole fill ([0aa60a1](https://github.com/stupside/castor/commit/0aa60a12fce22e12b0c2236d16d7350ef534c870))
* **log:** export logs over OTLP and tag every line with its cast id ([ddb01fe](https://github.com/stupside/castor/commit/ddb01fea15866c76779cc220bcd1a685bd96d133))
* **picker:** quit on q at once, without a confirmation dialog ([deeeed3](https://github.com/stupside/castor/commit/deeeed30a32cb20387ec9d4c8d4becafb15d20e1))
* **scraping:** add the resolver service ([ee64efc](https://github.com/stupside/castor/commit/ee64efcbc30eed4a01816a38d6f68f3f3ea8a161))
* **scraping:** improve player and iframe stream discovery ([eaa390e](https://github.com/stupside/castor/commit/eaa390e9753ccf64335386782cabf8c255761e94))
* show selected media details on playback devices ([c8e2666](https://github.com/stupside/castor/commit/c8e2666cbf6281cd12526a0a1f8426f3a606a2d6))
* **source:** read HLS segments ahead of ffmpeg, several at once ([eccd52b](https://github.com/stupside/castor/commit/eccd52b8a416095204722377239977cf93a39870))
* **source:** unwrap PNG segments for inspection and playback ([d005fc9](https://github.com/stupside/castor/commit/d005fc95c3825887ebb342b6614da1066e6a419b)), closes [#68](https://github.com/stupside/castor/issues/68)


### Bug Fixes

* **api:** bound concurrent device commands ([5fc20e4](https://github.com/stupside/castor/commit/5fc20e438bdbc219e8a2f91bb8a1af6c67b9cbf2))
* **api:** cancel target discovery and protect cast snapshots ([a5322d7](https://github.com/stupside/castor/commit/a5322d7f94af1f1846995eb246edd8a19200fa9a))
* **api:** cancel watch log forwarding ([ddab5e3](https://github.com/stupside/castor/commit/ddab5e3909954516d5801eea3d8d972dd4176db7))
* **api:** end a cast at once when it needs a device whose client has left ([5933d52](https://github.com/stupside/castor/commit/5933d5268d1696d5f272ab710e0e2cac3a8e52ab))
* **api:** give castor api server's shutdown its grace before it exits ([1d53b0f](https://github.com/stupside/castor/commit/1d53b0fa9e7040655c21a8e41579a12cdec50ee2))
* **api:** leave a cancelled extraction or ranking to connect's own code ([01edb63](https://github.com/stupside/castor/commit/01edb63d0eafa1685f701651ccdd191fb56e7f82))
* **api:** let only http and https links reach the server's browser and readers ([5784083](https://github.com/stupside/castor/commit/57840832889fc539a38c5048c2aa3aa580ba6f5f))
* **api:** refuse a cast that leaves its delivery unstated ([d8a31d2](https://github.com/stupside/castor/commit/d8a31d2421ce2065d7a9d669dbad33cae8e2bf9e))
* **api:** refuse a device that answers connect without its capabilities ([889556c](https://github.com/stupside/castor/commit/889556cc8e8feedc67ec8ed3ee1abcf11af444ca))
* **api:** reject reused device command IDs ([49aa56a](https://github.com/stupside/castor/commit/49aa56a3006649d1a8969227f7b2ef5db89617f3))
* **api:** send on the Drive stream from its handler alone, each send bounded by its call ([2133f21](https://github.com/stupside/castor/commit/2133f215ac676e719a4819cf0d79e2bf9bff0e7d))
* **api:** stop relaying a delivery's port once its listener closes ([357531d](https://github.com/stupside/castor/commit/357531d5764e19b717aab7262556a01f24c754e8))
* **app:** authorize server actions and propagate telemetry ([01e68ee](https://github.com/stupside/castor/commit/01e68ee832470fc325d7161c288a234102999a27))
* **app:** isolate watch credentials and cancel upstream streams ([5b301ab](https://github.com/stupside/castor/commit/5b301ab9ac48855e8ec5caf4909f29be78bfc599))
* **app:** model cast watch outcomes as exclusive states ([68d8e84](https://github.com/stupside/castor/commit/68d8e8428d8f001ba48adad731fd50d8cd8c4dce))
* **app:** recover device discovery and make cast controls resilient ([b1bfb98](https://github.com/stupside/castor/commit/b1bfb9866f5c6005e5517938be2990b3daf61b7b))
* avoid VideoToolbox SEI failure on re-encode ([83fd6f3](https://github.com/stupside/castor/commit/83fd6f3203587f60423251b7d35c1996ed9d89d1))
* **cast:** blame a delivery silent over castor's proven buffer on the delivery, not the source ([d0f7c1d](https://github.com/stupside/castor/commit/d0f7c1d628862ce45461a1a09d98c7641c6565c2))
* **cast:** end a playing cast whose renderer has had nothing to play for the stall window ([3cba9ed](https://github.com/stupside/castor/commit/3cba9edc79c215cad59c43750d7b1d263133f5b0))
* **cast:** fail a cast whose device ran out of media before the read finished ([26612aa](https://github.com/stupside/castor/commit/26612aa4bb022a668670573ff0504289447abd94))
* **cast:** give up on a delivery whose producer never writes its first artifact ([39b21cf](https://github.com/stupside/castor/commit/39b21cfa8540dbf3eb893ddcfecb967e4d1464e0))
* **cast:** hear sound where the source declares or requires it, and say when subtitles are skipped ([c642d18](https://github.com/stupside/castor/commit/c642d1883234e3152aa9ded0fbeec3cc5b8f1206))
* **cast:** honor ordered playback language preferences ([d3d7ba0](https://github.com/stupside/castor/commit/d3d7ba0adb0d9481e785e856a25f12fead190c25))
* **cast:** join the source read before teardown releases what it reads from ([c28b2d1](https://github.com/stupside/castor/commit/c28b2d1d3b0c621ac3d69090652e2d44cbc574ca))
* **cast:** judge a producer's growth against playback pace, not since the cast began ([01d034b](https://github.com/stupside/castor/commit/01d034b9b1ace0acba4ee0c8974699abf577aae1))
* **cast:** log a failed lighter rendition by the link castor read, not the rung's missing URL ([14fd3b7](https://github.com/stupside/castor/commit/14fd3b7af9a388fdc3659f0e184ce748dc1cfb81))
* **cast:** move to the next link when castor cannot read a timeline it follows ([c61962c](https://github.com/stupside/castor/commit/c61962cbb8c907d1dec6358b767a6fb2e4fd7f7c))
* **cast:** name a device that ran dry starved ([286f0b8](https://github.com/stupside/castor/commit/286f0b8e30398f5cfc460eba0072456e466385f0))
* **cast:** name why a device refused, and drop the prose behind it ([173d094](https://github.com/stupside/castor/commit/173d0944110b8bcd983f21addc9fbedd585536e2))
* **cast:** serve instead only when the renderer was handed the source ([c771bdf](https://github.com/stupside/castor/commit/c771bdf12ae5ad33013727c8179228ac87230927))
* **cast:** transcribe only a read sure to carry sound ([0cd56dd](https://github.com/stupside/castor/commit/0cd56dddbe170435425a873d1028659e88358067))
* **cast:** validate served media and measure HLS renditions ([5aa144d](https://github.com/stupside/castor/commit/5aa144dcd83780571cbd892bcd21a34e63e6fdaf))
* **chromecast:** cancel blocked writes ([1821014](https://github.com/stupside/castor/commit/18210147523b7e326e3be9bc8d0d2fd38387b5f3))
* **chromecast:** end the cast as gone when the Cast connection drops ([79fa899](https://github.com/stupside/castor/commit/79fa899ec64ec2bd1998aa0be1c7e74f80572f7d))
* **chromecast:** match LOAD status to the requested stream ([6d4f823](https://github.com/stupside/castor/commit/6d4f8230b47120f178b6c4c9d7aa2ef57e6f1f1d))
* **chromecast:** reject LOAD replies without media status ([e15ef25](https://github.com/stupside/castor/commit/e15ef2565a80d7c99202d63e76407de43e7bbb6d))
* **ci:** restore release PR checks ([25571b5](https://github.com/stupside/castor/commit/25571b5a715d8cafc4da58e97d9e3870bdf008d7))
* **ci:** update Staticcheck for the Go toolchain ([43b9cdd](https://github.com/stupside/castor/commit/43b9cdd2cec334ea85c4d30c8045cba064605436))
* **client:** leave the drive when an answer to the server is lost ([6691044](https://github.com/stupside/castor/commit/66910441e9cba8b729ca12a23135f0d2163c6190))
* **client:** lend the LAN only the server's relay route, never its API ([4929538](https://github.com/stupside/castor/commit/4929538b032701fd63d4697c4b634008d4f69d69))
* **client:** open the LAN relay for the first play that needs one, never to close it ([eebaff4](https://github.com/stupside/castor/commit/eebaff464055dc3234c62b3a7e55b30a8c98d519))
* **cli:** isolate genre drafts and discard stale browse results ([359a161](https://github.com/stupside/castor/commit/359a1618448dfd38a5ae8d1a917f621ead1d7c68))
* **cli:** keep forwarding buffered logs ([b2ce63b](https://github.com/stupside/castor/commit/b2ce63b0b988968bd718617878a355879d0301fa))
* **cli:** load only configuration needed by each cast action ([ecef142](https://github.com/stupside/castor/commit/ecef142022e5ba0b821ddaefe44b13c0ea438d0e))
* **cli:** preserve grouped log redaction while holding output ([37f1ff1](https://github.com/stupside/castor/commit/37f1ff18343a093d09b8ada6fa6a358167bebd75))
* **cli:** refuse to start when the log file cannot be written ([eab1c61](https://github.com/stupside/castor/commit/eab1c614050ee340dec0ddc0311c32747a425aec))
* **cli:** require cast arguments and preserve configured scan endpoints ([805f977](https://github.com/stupside/castor/commit/805f977b7e0c8fd63760a42996416891e8b98436))
* **cli:** stop casts when their status watch breaks ([666ffe4](https://github.com/stupside/castor/commit/666ffe403ea60de00fb3765529deb715d0956b9c))
* **cli:** stop q quitting the drilldown and tidy the browse loop ([a7ce7c2](https://github.com/stupside/castor/commit/a7ce7c27c37e3c052bae9d1900df3238bc446763))
* **cmd:** stop a cast only on Ctrl+C, not when its watch ends ([26c42f3](https://github.com/stupside/castor/commit/26c42f3ff2ba475d274e14a121e7ece05ada3bd5))
* **cmd:** stop the cast and release the drive whatever ended its watch ([13f97f2](https://github.com/stupside/castor/commit/13f97f207e5aada69451ad7e0f632804ad88ee51))
* **cmd:** take an episode's season and number as unsigned, not wrapped from negatives ([5dde342](https://github.com/stupside/castor/commit/5dde34269c5bb4b7317ee508fdf3ceebf496cd48))
* **config:** reject unknown keys in owned sections ([bad50e1](https://github.com/stupside/castor/commit/bad50e17a090621b358d3915a6ad260290e9f947))
* **config:** report unreadable files ([8a33e26](https://github.com/stupside/castor/commit/8a33e2622e8b606d3bdbd26185b1f4af2538a0e1))
* correct HasVideo doc comment for lint ([d0cc2f0](https://github.com/stupside/castor/commit/d0cc2f0b9d5e54a3edf814819d23c125201dd444))
* **dash:** bound timeline repeats by availability and period end ([9a1806a](https://github.com/stupside/castor/commit/9a1806af1f6ba08bb0fd424ecd43a088e6fe834d))
* **dash:** never give the last indexed segment a negative length ([5faa050](https://github.com/stupside/castor/commit/5faa05032eae470a126a7890383914d73f28539a))
* **deps:** bump golang.org/x/net to v0.60.0 ([674a355](https://github.com/stupside/castor/commit/674a3552c45fd8ff4eaf960675db1bcaaeade078))
* **device:** echo what the device advertises and notice when it stops ([4858511](https://github.com/stupside/castor/commit/4858511611f52e133e14b1caaf7f67633b76fa8f))
* **device:** judge a renderer gone by how long it went unanswered, not how many polls failed ([56ceb1c](https://github.com/stupside/castor/commit/56ceb1c4205f072921c1a92dfe47b6784ecadac5))
* **device:** preserve poll cancellation ([d42e3ff](https://github.com/stupside/castor/commit/d42e3ff97d8f369316b71bac7c0577fb29a2216d))
* **devices:** bound device connections by the network timeout ([7acfb4b](https://github.com/stupside/castor/commit/7acfb4bb21865b24d85edfe90a1625459887f2cd))
* **dlna:** bound pinned SSDP searches ([423c4ce](https://github.com/stupside/castor/commit/423c4ce0806d206592e763fa657b8092b77e0372))
* **dlna:** cancel pending discovery ([946842a](https://github.com/stupside/castor/commit/946842aa08fdc902358b4f303377da732e76dcdb))
* **dlna:** confirm playback after a timed-out Play request ([eaefa19](https://github.com/stupside/castor/commit/eaefa19d130c7c0ca9d17f483075f05b9ddce3ff)), closes [#68](https://github.com/stupside/castor/issues/68)
* **dlna:** deduplicate advertised playback capabilities ([9711efd](https://github.com/stupside/castor/commit/9711efd6d1221109f51b90a1c5408a962c74c17a))
* **dlna:** retain conservative playback when capabilities are unavailable ([570ce08](https://github.com/stupside/castor/commit/570ce089f5c1509d1a16b5473adab1dbc3d414bd))
* **docker:** use host networking for LAN discovery and media delivery ([33f5577](https://github.com/stupside/castor/commit/33f55776a55222da034d3b2cc7fb8f6bd5a58b70))
* **extract:** bound each page and the snapshots taken of it ([f7391be](https://github.com/stupside/castor/commit/f7391be1d5e901d7d8ce0782b820a270b0d8c971))
* **ffmpeg:** count a kill as castor's only while ffmpeg is still running ([3861fde](https://github.com/stupside/castor/commit/3861fde2d678bb3e0605add11da1ee584c7ab663))
* **ffmpeg:** detect HLS demux I/O errors as incomplete reads ([60d1a6a](https://github.com/stupside/castor/commit/60d1a6a72c519864005b6ea57a63123cd60643f2))
* **ffmpeg:** limit input protocols to the network ones a source is read over ([409d4b7](https://github.com/stupside/castor/commit/409d4b7dc0d4dfd7eef1d06b19df0e0b61baf6c5))
* **ffmpeg:** tell castor's own kill from a failure on Windows ([4ba63d6](https://github.com/stupside/castor/commit/4ba63d66a2f4b76aeffaa957346bd1287c0992cd))
* **follow:** answer a segment whose origin broke before its first byte with a bad gateway ([89227ae](https://github.com/stupside/castor/commit/89227ae64353bf6d44e7fdcbe0d2a55e5045213c))
* **follow:** let an empty first window leave the repackaging choice open ([8edd6ef](https://github.com/stupside/castor/commit/8edd6ef45f7b4ef035680da7490632c6c3f7960c))
* **follow:** read a timeline's first window again after a passing failure ([1ba319c](https://github.com/stupside/castor/commit/1ba319c50be49c22e2c3fd4eb2acf476440de197))
* **health:** describe stalled reads accurately ([9fdb890](https://github.com/stupside/castor/commit/9fdb890a1071d3a695f158a29f0bbdfd3dc40218))
* **hls:** accept short hexadecimal AES initialization vectors ([cf6e2f0](https://github.com/stupside/castor/commit/cf6e2f0c9889c2dce942f859055b779d41d8f65c))
* **hls:** honor receiver segment envelope capabilities ([c3ea12d](https://github.com/stupside/castor/commit/c3ea12d1a49b760ca1049253408489aeada6d944))
* **hls:** open each segment on its own connection ([1aff98c](https://github.com/stupside/castor/commit/1aff98c798f60195fa74873c1b0a2945675d54aa))
* **hls:** read an init BYTERANGE without an offset from the first byte ([2bb368f](https://github.com/stupside/castor/commit/2bb368f13b973c340fccfa5d5ea95a060174acfa))
* **hls:** relay original fragments when no repackager is available ([99d45ea](https://github.com/stupside/castor/commit/99d45eacdbfc70d3b1ce25a0a8a67e01d65020af))
* **hls:** release cancelled callers waiting for shared resources ([9684094](https://github.com/stupside/castor/commit/968409467c48045f71416e55e6ef8f1fb506c910))
* **hls:** restore direct playback for ordinary segments ([eb4ab78](https://github.com/stupside/castor/commit/eb4ab78393a6892c740c6026914519f75265134b))
* **hls:** retain settled renditions and reject protected companion audio ([9a4a1ce](https://github.com/stupside/castor/commit/9a4a1cecf720335c95d1006e0cbbeae9f37cdc4e))
* **hls:** send framed responses to ffmpeg readers ([f4e2e06](https://github.com/stupside/castor/commit/f4e2e069cc5d8471577fae4373d9efafb0193698))
* **log:** stop logging the healthy watch gate and ffmpeg's routine lines ([8faae55](https://github.com/stupside/castor/commit/8faae55519ab291b8626d9eb9c6a3d0f08a0ee16))
* **media:** enforce segment write deadlines and count delivered bytes ([f60b8f7](https://github.com/stupside/castor/commit/f60b8f78beee012f45144b0a9c2c9a46e366bd59))
* **media:** play audio-only streams without a video encoder ([fb27dcd](https://github.com/stupside/castor/commit/fb27dcda918ab8b9876f6416ce0dd5d43c0c2c60))
* **media:** respect advertised audio channel limits ([c693e54](https://github.com/stupside/castor/commit/c693e54d155dc81e52009834e59799b6c6219c74))
* **mediaserver:** bound origin document reads and drain a stalled progress feed ([21aea51](https://github.com/stupside/castor/commit/21aea51709a5930f444ff1699ba477bbb91417dc))
* **media:** support audio-only handoff and absent tracks ([2309ff0](https://github.com/stupside/castor/commit/2309ff0585a2e5d6200e267cba238dc060ecdf89))
* **media:** try another delivery when preferred encoding is unavailable ([a38c523](https://github.com/stupside/castor/commit/a38c523647e5f76674c4deb7289436f743526803))
* **probe:** read pixel component depth without confusing format layout ([dbb7249](https://github.com/stupside/castor/commit/dbb724973599e87ed8ff3dffc35425318d60e910))
* **rank:** admit a short stream as a last resort ([9524ca1](https://github.com/stupside/castor/commit/9524ca1ecdc60819e909b267743846f20f5f473f))
* **replay:** keep credentialed stream paths distinct through recovery ([fc3e559](https://github.com/stupside/castor/commit/fc3e5599f029f233caf82b430e1a424483f8835f))
* restore discover toggle and separate test environment ([bd5826b](https://github.com/stupside/castor/commit/bd5826b05039cec0c6c2c7deabed8128231b8db8))
* **roku:** refuse unsupported containers ([9179dc7](https://github.com/stupside/castor/commit/9179dc78ec9c3c2885fb8d05e109f575c4999c7b))
* **roku:** reject malformed app lists ([3483fb4](https://github.com/stupside/castor/commit/3483fb40cd99f6581c2cd9d13b3837360061ef31))
* **roku:** reserve discovery time for device names ([ac2e29b](https://github.com/stupside/castor/commit/ac2e29b325a72aad55a303430e4d06582f660220))
* **roku:** validate app lists and support IPv6 endpoints ([8a1472f](https://github.com/stupside/castor/commit/8a1472faedb9127e6dc894bbef59529af716ec3c))
* **rpc:** validate requests and downstream responses at service edges ([c4d056f](https://github.com/stupside/castor/commit/c4d056f78670b742ab5e424a65e75137af09c91b))
* **scraping:** bound browser capture and preserve redirect credentials ([8263017](https://github.com/stupside/castor/commit/8263017212db59b54f1fce79e8c30e5840b3e517))
* **scraping:** parse bounded manifest evidence and inherited DASH URLs ([26f27d4](https://github.com/stupside/castor/commit/26f27d4907a2296237b5d2ed7436ffa3ebbeae06))
* **scraping:** preserve resolver cancellation status codes ([b2233cf](https://github.com/stupside/castor/commit/b2233cf32a1660db863b9975db14d992b6393c88))
* **scraping:** use backward capture iteration for go fix ([37c3a85](https://github.com/stupside/castor/commit/37c3a85ae3a68af17dcb14f884459e7232cec7ad))
* **source:** follow re-signed segments once and bound what is buffered ([e55ae42](https://github.com/stupside/castor/commit/e55ae42b77b55899b52ee5ae24af10c3aafec2c5))
* **source:** preserve cancellation during stream ranking ([d8bd752](https://github.com/stupside/castor/commit/d8bd7529574f172df2046714114e605290f5ee43))
* **source:** preserve unresolved playlist failures through completion ([a28a726](https://github.com/stupside/castor/commit/a28a72635018ea4e843190ad6861f7050acfac1e)), closes [#68](https://github.com/stupside/castor/issues/68)
* **source:** report fallback from selected audio track ([a27cf0d](https://github.com/stupside/castor/commit/a27cf0dbf3cc272c3264f7042c1102a18f5bb45c))
* **source:** retain declared codec levels for decoder limits ([b0d08e9](https://github.com/stupside/castor/commit/b0d08e90e78ac4967b7423f1c44c31ecbf3ff387))
* **source:** validate media ranges and abort truncated segment responses ([694e7b9](https://github.com/stupside/castor/commit/694e7b98093a837ba6a881f3d0d664077e36edb3))
* **streaming:** follow production for open byte-zero live ranges ([e5456f1](https://github.com/stupside/castor/commit/e5456f1ff4ad2c69525ef5bce98ca0693f2cace0)), closes [#68](https://github.com/stupside/castor/issues/68)
* **subtitles:** ask for a language in whisper's own codes ([3535589](https://github.com/stupside/castor/commit/353558928bbd586089041b4aff5ca35ccbfe1416))
* **subtitles:** select multilingual models and cancel transcription safely ([656bbe2](https://github.com/stupside/castor/commit/656bbe2b62a1adf7824c8c73d6eb90b3e7c67961))
* **timeline:** count a seam in the discontinuity sequence when its tag scrolls off ([467513b](https://github.com/stupside/castor/commit/467513bfa859802794e9ca5230bda7760125d769))
* **timeline:** never republish a segment a lagging edge lists again, however long ago it was trimmed ([4c7b729](https://github.com/stupside/castor/commit/4c7b72976ef178bc9309d51e51d27db406b9f987))
* **tmdb:** honor proxy settings and dial timeouts ([4ef029f](https://github.com/stupside/castor/commit/4ef029ff9d405f7e6cc1c5532b6e85fe75267920))
* **transcode:** declare a seamed program's discontinuity threshold once, before its inputs ([a0808b2](https://github.com/stupside/castor/commit/a0808b2be39ac82eb4d9075bd981391a0fc274af))
* **transport:** drain work after listener failures and release startup ports ([ab17a37](https://github.com/stupside/castor/commit/ab17a37961b0caf533027adb69a1a4fc976e7b3a))
* **transport:** keep bearer credentials on the configured origin ([037bbdc](https://github.com/stupside/castor/commit/037bbdc809a3c1da766a95777bc0d6cd460eabbc))
* **whisper:** verify downloaded models against pinned SHA-256 ([ccd981d](https://github.com/stupside/castor/commit/ccd981d62aad7df8b6ba269e215768411588418f))


### Performance

* **media:** avoid cloning probe data ([c55afc1](https://github.com/stupside/castor/commit/c55afc11a4a5a211cfc203893c1b631e3837e846))


### Refactors

* adopt newer standard library idioms ([8c16ddb](https://github.com/stupside/castor/commit/8c16ddb7acb986fd46c06f4233423eebc2067ab2))
* **api:** build a session's watchers with it, not on the first subscribe ([1733384](https://github.com/stupside/castor/commit/1733384f0e89d0745f75e935132a76fd73ff28da))
* **api:** build the server relay's proxy once, reading the route's values per request ([3231f03](https://github.com/stupside/castor/commit/3231f035f1d73df28ca97a572c0c0c5101bd0f88))
* **api:** carry a stream's headers as one value each ([60506ed](https://github.com/stupside/castor/commit/60506eda207d7bc518ec0d24bf1f94af5b94b815))
* **api:** count in unsigned integers wherever nothing can be negative ([17b9c42](https://github.com/stupside/castor/commit/17b9c42b3c460ba6040329177fbc9900cbac0275))
* **api:** drop rules and comments the contract already states otherwise ([81acb5f](https://github.com/stupside/castor/commit/81acb5fbe04f227450f92cc1839c30d88ca1f0f0))
* **api:** hold a cast's lifecycle in a looplab/fsm machine ([11a4638](https://github.com/stupside/castor/commit/11a4638ec67c8077aecff43061db650afddcb459))
* **api:** hold to the contract what a client sends, and say less in its comments ([7922754](https://github.com/stupside/castor/commit/7922754c230a0c839a5d7e374353bea6af0b4d72))
* **api:** leave a watch's log level unset to ask for none ([1f35f2e](https://github.com/stupside/castor/commit/1f35f2efd58e5712c97b4ef7580aee5fccb1c20e))
* **api:** lend a cast one device, so its commands carry no handle ([0e8be23](https://github.com/stupside/castor/commit/0e8be239f313e1b54d7a014059caeeb2006caa62))
* **api:** lend a device with whether it fetches for itself, not a whole profile ([d417fac](https://github.com/stupside/castor/commit/d417facd146f0d257fed919c16b18418e1f9ec6d))
* **api:** name the cast RPCs Start and Stop, as every other RPC names its verb alone ([fd27212](https://github.com/stupside/castor/commit/fd272128d0139769e194fdb86126ab9e7a1791ff))
* **api:** name the device families after what they hold ([b74f196](https://github.com/stupside/castor/commit/b74f1967194f2be47f1b26c1a66d14f768d53488))
* **api:** own remote sessions and join device observers ([2628e52](https://github.com/stupside/castor/commit/2628e521eb639450626afe366d981407b3c0a01e))
* **api:** read a watch's end one way, and name every refusal the server makes ([e12281a](https://github.com/stupside/castor/commit/e12281ac4276f9e2a165d2b8b256cbf8a4e8e7a9))
* **api:** reduce a cast's status to its counters ([4e609c4](https://github.com/stupside/castor/commit/4e609c4c601f6bdc85be5166268ad3f06662a510))
* **api:** wait for a device for the undriven constant, not a field set to it everywhere ([47463f7](https://github.com/stupside/castor/commit/47463f73d3d05e7a20091a9f27ce76ce40c3012a))
* **app:** drop the unused casts slot ([1710e81](https://github.com/stupside/castor/commit/1710e818db97f08384a2d10704a1f8f2b96ba825))
* **app:** keep one cast submission path ([3a42330](https://github.com/stupside/castor/commit/3a42330fcb5964c6c564e34c6ac1dc2c9636edd8))
* **app:** query casts directly ([c4045f1](https://github.com/stupside/castor/commit/c4045f111344e07ed9278214084388ecd689e5fd))
* **app:** use one API transport ([770d402](https://github.com/stupside/castor/commit/770d4023d0cf3ab049fcb5f5788d6e6dbb7ab278))
* **browse:** read fields directly instead of through one-line accessors ([0015a6b](https://github.com/stupside/castor/commit/0015a6b90a94bc8580af2642ad841496456dbae3))
* **cast:** cast straight through attempt, and drop what only tests or nothing reached ([a7b5918](https://github.com/stupside/castor/commit/a7b5918c7900e946fdb29fdbd69ae4a8dc6db46e))
* **cast:** coordinate typed preparation and readiness stages ([05279b2](https://github.com/stupside/castor/commit/05279b2bad4ec6729f849bfdfaf6c4c5e4e44527))
* **cast:** declare one Listeners port, in deliver, and open every delivery through it ([6153550](https://github.com/stupside/castor/commit/6153550bbdba71337ec14cd177999f8833d414d0))
* **cast:** finish renaming read plans to fetch plans and candidates to streams ([0a4f93c](https://github.com/stupside/castor/commit/0a4f93c5fbbc8081aeb86f50731dc4d177a4ad1d))
* **cast:** fold single-file packages into their parents ([bac478c](https://github.com/stupside/castor/commit/bac478c858cfcd5494f2f6b3ea0aad5562284c26))
* **cast:** leave a slow source to the device ([dc584de](https://github.com/stupside/castor/commit/dc584de7a9f494b023920a4b63931be034536e7c))
* **cast:** name read and watch by what they decide: fetch and health ([4d78b0a](https://github.com/stupside/castor/commit/4d78b0a5a2570b6b68d468a5372506bbafde0301))
* **cast:** open deliveries through a Listeners port, under the cast's context ([6f4764c](https://github.com/stupside/castor/commit/6f4764c72ae5d8be7be80b7ce03fd6712196d402))
* **cast:** run an attempt on the values its steps return, and drop the indirection around it ([9418e0f](https://github.com/stupside/castor/commit/9418e0f63d007944e9ec6a1ce9fa5bcec816b205))
* **cast:** stand in a Turns nobody hears once, not a nil check at each turn ([f1e3a16](https://github.com/stupside/castor/commit/f1e3a16d5942b9046941bca94571ada397a608e3))
* **client:** leave the contract's rules to the server, and say plainly when it refuses ([462167a](https://github.com/stupside/castor/commit/462167a8cf2090d2b57d360def9c65f9fcb0623e))
* **client:** name the LAN address port Address, as one address it is ([f3874ea](https://github.com/stupside/castor/commit/f3874eac920574b66c2712446b60053f347f7b89))
* **cli:** name and group the castor command line ([95463fa](https://github.com/stupside/castor/commit/95463fa17076631785f83d3436cd7c9f001bcbb3))
* **cmd:** build the missing TMDB key error with errors.New, having nothing to format ([758372a](https://github.com/stupside/castor/commit/758372a08917291719b6746ecb53abec38628371))
* **cmd:** load config with a method, and inline the forwarders around it ([6fa2ee8](https://github.com/stupside/castor/commit/6fa2ee8f1f8c8afca9e4fc7cdb938d11ccda929d))
* **config:** connect through remote.url and serve as castor server, one section each ([0fb2839](https://github.com/stupside/castor/commit/0fb283926af0eecf9dd0ce646d741ca768ee1047))
* **config:** group service settings and reject unknown keys ([88cc8ea](https://github.com/stupside/castor/commit/88cc8ea7fdf4a880efd5de13d8873de24fcc1d26))
* **config:** identify a link with its cast's own resolver ([206865a](https://github.com/stupside/castor/commit/206865a1c8dfa80dfe55d7b6be7e8ddae93abf82))
* **config:** iterate struct fields with reflect iterator ([061725c](https://github.com/stupside/castor/commit/061725c28d59b6c6abf47cf429d4e3f9b3902884))
* **deliver:** open deliveries on their Opening, with what is written where passed alongside ([adf9f61](https://github.com/stupside/castor/commit/adf9f61a3dcf9d7770be6c6b0b0f63bc9b5d649b))
* **device:** drop what renderers and screens carried for nobody ([e8bea2b](https://github.com/stupside/castor/commit/e8bea2b69ffc27b381c888682ee1158ee4a6df21))
* **device:** hold constants every caller passed as parameters ([6a6ddad](https://github.com/stupside/castor/commit/6a6ddad593b61725150b4060daf40c8e9de8f93a))
* **device:** separate discovery from device control ([84eefac](https://github.com/stupside/castor/commit/84eefac9c817824fb63d73aec859fc31ef2134a4))
* drop the probing and extraction layers that held nothing ([3991e73](https://github.com/stupside/castor/commit/3991e73aca030f483539836ada7e869558e7cdcd))
* drop the standalone castor-api and castor-media binaries ([5c74b40](https://github.com/stupside/castor/commit/5c74b4013109cc640da4f956cd58a503a7856622))
* drop what media and subtitle carried for nobody ([6709ecc](https://github.com/stupside/castor/commit/6709ecc44848f60de794b6ec5a8f4cc6372bd18b))
* **e2e:** drop unused bookkeeping ([2af6c1f](https://github.com/stupside/castor/commit/2af6c1fba30c3151c8a83108d85901563d71a3cb))
* **execute:** call what an attempt keeps its files in a directory, not a one-field workspace ([68da4a9](https://github.com/stupside/castor/commit/68da4a9ece635fffec7b0689c0e54661ef39dda5))
* **extract:** drive the page and parallel extraction without single-use callbacks ([8a77d75](https://github.com/stupside/castor/commit/8a77d75f28ae02002150d222d6dd7da07fcc9c5d))
* **extract:** log what a page capture finds under the extraction's context ([53bc091](https://github.com/stupside/castor/commit/53bc091c99540569994e2a7aba1a66a7fa5aa12f))
* **ffmpeg:** centralize startup resource cleanup ([28d85db](https://github.com/stupside/castor/commit/28d85dba6b46272e90f85cdac8893aa9173c65e8))
* **ffmpeg:** use inherited pipes for Unix side outputs ([3ef689e](https://github.com/stupside/castor/commit/3ef689eb5cb29bb14c137fea5d79ede230743a9e))
* file each screen with what it picks: titles and devices ([27c3e62](https://github.com/stupside/castor/commit/27c3e62210f2acf3ea2ea2ed4d003f2159a50d2a))
* give the API server and the media server the same shape ([160ddb6](https://github.com/stupside/castor/commit/160ddb60eccc631e9584a87a97c944812c490a98))
* **hls:** centralize observed source compatibility ([2824043](https://github.com/stupside/castor/commit/2824043b3d0a48ac7da000c1dd9d0c06b0cbe054))
* **hls:** separate AES decryption from fetching and bound key reads ([ae57b52](https://github.com/stupside/castor/commit/ae57b52e631ff546e0582c0eb91b78fc5c993404))
* keep both servers' casts in one shared registry ([c7d478d](https://github.com/stupside/castor/commit/c7d478dcde91cf93ba744a4f30a77d791ac4e30c))
* make the TUI and the process plumbing part of the binaries ([77ce80e](https://github.com/stupside/castor/commit/77ce80e656cfd9493aff38c71d0466c55006b79a))
* **media:** bind probe evidence and preserve explicit tracks ([5897b74](https://github.com/stupside/castor/commit/5897b74e259098254db21b7127f95fd6cb96bfc6))
* **media:** collect a program's header names in one place ([ef39734](https://github.com/stupside/castor/commit/ef39734005606437b46c06936339c85a8659f107))
* **media:** contain cast lifecycles and publication ownership ([c55f264](https://github.com/stupside/castor/commit/c55f264e5cab97b01895ab0630bd66f4fb62b13e))
* **media:** drop extraction leftovers ([0788a14](https://github.com/stupside/castor/commit/0788a14052bc2f82225c978b75c860ad80f9c0b6))
* **media:** isolate segmented source decoding by format ([37a0826](https://github.com/stupside/castor/commit/37a08260dd6b72802f44ce6208cd0125c4d64579))
* **media:** name and group the ffmpeg, probe, media and subtitle tools ([ad6d943](https://github.com/stupside/castor/commit/ad6d943b61bda7d94809abb29ffc9a67f9b56ca7))
* **media:** name and group the source and extract packages ([6c68eb5](https://github.com/stupside/castor/commit/6c68eb5cec6cffcc3ffdf5b32ddb4d8a682f02d9))
* **media:** name the cast runtime after what it does ([ab2ff64](https://github.com/stupside/castor/commit/ab2ff6496c814820f114b13330b75fe12374db7b))
* **probe:** inline input tolerances ([066f1eb](https://github.com/stupside/castor/commit/066f1eb809e1c5ae7813d4cd31a44b6826113db5))
* **proto:** name subtitle preference branch for its policy ([af8c784](https://github.com/stupside/castor/commit/af8c784a78e0611c3342bbadf8f41ea6b9776563))
* **proto:** remove compatibility reservations and compact fields ([7a967cb](https://github.com/stupside/castor/commit/7a967cb24ef6d0e7cdc9f61c91ffe90d1482ab69))
* **proto:** type video support by codec ([7683110](https://github.com/stupside/castor/commit/7683110fd52da27edb731566664daba6f535e144))
* **rpc:** isolate playback contracts ([9bf0c3e](https://github.com/stupside/castor/commit/9bf0c3ee029aaae9cfdc2db5104fc97c60f037bb))
* **rpc:** split audio and video codecs ([75b4f24](https://github.com/stupside/castor/commit/75b4f243b1381d34372698326926973c580c661a))
* **rpc:** type device families ([0896152](https://github.com/stupside/castor/commit/0896152658b21797a9eb82c89c348207d28c21ed))
* **rpc:** type stream metadata ([68ba23d](https://github.com/stupside/castor/commit/68ba23d11d0ff45d64095b13cad4e382dc7d3bf0))
* **scraping:** emit generated candidates and keep document inspection private ([684f16f](https://github.com/stupside/castor/commit/684f16f70e19f8d2fee76843ffd637d0e6dae5b0))
* **screens:** move the browser, the picker and the logger to Charm v2 ([7b977e4](https://github.com/stupside/castor/commit/7b977e459c00328de0e7eb42fe092e94109b6f0c))
* **screens:** name the bar colours, draw every list with one delegate, ask the background once ([20b0c58](https://github.com/stupside/castor/commit/20b0c58a87f898f98b044ddb43f8f6ce3e246de1))
* **source:** call a found link a Stream, as everything that hands it on does ([aa29554](https://github.com/stupside/castor/commit/aa29554f8157fe04dc6611d292e0cc2717ead2bd))
* **source:** give each port only what its implementations use ([e7eef87](https://github.com/stupside/castor/commit/e7eef874021d2a21c83450e5a7c683322b130526))
* **source:** identify a link without a header nobody passes, and inline config's one-line helpers ([ceb8b49](https://github.com/stupside/castor/commit/ceb8b49308d57418ebd7c3a70414eb7e7f6b4d5d))
* split castor into sealed media server, API server and TUI tiers ([10224d5](https://github.com/stupside/castor/commit/10224d5bf322409c48b0ea029177b369209ce703))
* start both servers through transport.Listen and transport.Loopback ([5137b23](https://github.com/stupside/castor/commit/5137b23f2767cea8e72b058ad57b28e888b60241))
* **subtitle:** name subtitle.Word and ensure the VAD model directly ([c431374](https://github.com/stupside/castor/commit/c4313747b477971043c2258a248245f64b3e8e09))
* **subtitles:** encode transcription within enabled selection ([0ad24d0](https://github.com/stupside/castor/commit/0ad24d0f5aac26a54f9f5d942a297a524462b60d))
* **test:** simplify recovery doubles ([e3d7014](https://github.com/stupside/castor/commit/e3d70140ef5df3d4e55f9fc7c506c3e364f9c225))
* **tmdb:** read release dates directly ([06aa66c](https://github.com/stupside/castor/commit/06aa66c17ad1a3c658e7f5e444a0296b33d50169))
* **transcode:** use output tuning directly ([20e487a](https://github.com/stupside/castor/commit/20e487a94beefb335b526c42c751d853f16ddf11))
* **transport:** split serving and the token rule out of transport.go ([10bfe91](https://github.com/stupside/castor/commit/10bfe915326d452a0404035c5437b84658a20b7a))
* unexport what no other package reads ([9da3c09](https://github.com/stupside/castor/commit/9da3c09fc2bcbf16788040ea26252619ff621da9))


### Documentation

* condense architecture and show cooperating state machines ([9639305](https://github.com/stupside/castor/commit/9639305c57f2f020eb07af858b0c746d48eec871))
* **config:** say subtitle burn-in reaches DLNA only ([9f746f2](https://github.com/stupside/castor/commit/9f746f28798aee7152b74138d058d5c5988212ba))
* **container:** say what the package describes ([4f17f03](https://github.com/stupside/castor/commit/4f17f03532488b51f7c7211f71c78b04970db1a4))
* describe lifecycle ownership and shared media publications ([d0ac6e5](https://github.com/stupside/castor/commit/d0ac6e5375d8bdd58252df6dfdca1a8208740756))
* describe observed HLS handoff boundary ([11860b0](https://github.com/stupside/castor/commit/11860b020d6510c376a7dbd2b81ca0ddae6ab32f))
* explain format owned segmented source reading ([0675f36](https://github.com/stupside/castor/commit/0675f36e184511f517e4f2f87f0ed5bf42329adc))
* explain how castor works inside in ARCHITECTURE.md ([b8f9b8f](https://github.com/stupside/castor/commit/b8f9b8f0c1a6a776ff2c58b57afc080076392208))
* prepare Castor 2.0 migration ([#69](https://github.com/stupside/castor/issues/69)) ([75bf500](https://github.com/stupside/castor/commit/75bf5001f3ce9f941103897288349c4b3879e52b))
* **readme:** cover using castor, and leave its mechanics to ARCHITECTURE.md ([b7c3a9d](https://github.com/stupside/castor/commit/b7c3a9d775dd210dc30673a6c040d8271b13f947))
* rewrite ARCHITECTURE.md around tiers, topologies and boundaries ([d9a3235](https://github.com/stupside/castor/commit/d9a3235a52c938f6be5cac59467c4d59ca854ab6))
* say what the media server model does where comments and SECURITY.md still told the relay's ([4dafe9a](https://github.com/stupside/castor/commit/4dafe9a2c446a100537f3fa687bd5b9c8afd99a6))
* **security:** say castor serves plain HTTP and to terminate TLS in a proxy ([49394b6](https://github.com/stupside/castor/commit/49394b6999ecc66bdd0cacc0cc1fa00966d9ac9b))
* streamline setup and usage in README ([8edc2f6](https://github.com/stupside/castor/commit/8edc2f67ebde05552c6e6b309db4afc48bcb784f))
* tighten the readme, contributing and security guides ([d0c3e38](https://github.com/stupside/castor/commit/d0c3e38b5f10bfd41530824736610e6ccfdadc04))
* **transcode:** say the splice timestamp threshold holds for every input ([7ee3d01](https://github.com/stupside/castor/commit/7ee3d01decf04bfd4ce79aaa7f5bfc076581d3cd))
* trim the service guides ([bcc0ef3](https://github.com/stupside/castor/commit/bcc0ef371aa649ef57db2c8e4fd7daa369aeedff))


### Build System

* **app:** drop unused headless UI ([1db6f8e](https://github.com/stupside/castor/commit/1db6f8e376ec21e0af1698311ef4ef404e9b2d4a))
* **app:** validate the web app in CI and wire the Tilt environment ([b64ee08](https://github.com/stupside/castor/commit/b64ee0818533c7e2b336acd3ca76800934ec7930))
* **deps:** bump Go to 1.27.1 and the direct dependencies ([83ea245](https://github.com/stupside/castor/commit/83ea245d65ee711a3c6792f4a104236c38a0eb99))
* **deps:** bump mp4ff, koanf and teatest, and keep node_modules out of ./... ([a201352](https://github.com/stupside/castor/commit/a2013528898c330234f91d0f0c245c18a619bed4))
* **deps:** bump whisper.cpp to v1.9.4 ([a1f75e3](https://github.com/stupside/castor/commit/a1f75e38bbe81a4dbe5b326dc44ae3c7503fed42))
* **docker:** limit the build context ([c004c67](https://github.com/stupside/castor/commit/c004c67e0ecd508830a5045cbe2bc54c8c085deb))
* drop the tooling that did nothing ([b563df3](https://github.com/stupside/castor/commit/b563df3876a4a7711059e0b069a952a394ea8c1c))
* move to Go 1.27 and the latest dependencies ([f4056b8](https://github.com/stupside/castor/commit/f4056b8617b1eda524916a8927e413f4a778348d))
* **proto:** drop compatibility checks ([3d88d82](https://github.com/stupside/castor/commit/3d88d82495fcdca866ad6f3170f996a28d07d22d))
* **release:** rename the cask script to brew.sh ([e3151ed](https://github.com/stupside/castor/commit/e3151ed9de224e2ba67b0c5b3ca4c30810d22a38))


### Continuous Integration

* bump download-artifact, setup-node and upload-artifact ([becf454](https://github.com/stupside/castor/commit/becf454eefc42dc5bcfea67e662ad2ab1ad25db8))
* bump the action pins and lint tools, and gate on go fix ([fb187c8](https://github.com/stupside/castor/commit/fb187c8406f24ed6b2eb608f667da40742978b7f))
* check only first-party packages ([2e91984](https://github.com/stupside/castor/commit/2e91984a323b37d3fee45419e3cb3a36893b5b97))
* install ffmpeg 7.1 and keep go's download noise out of the deadcode gate ([3c491f1](https://github.com/stupside/castor/commit/3c491f169afadffef2e51a6a3f82ef156a467a9b))
* leave the e2e suite out of the test job ([44ac704](https://github.com/stupside/castor/commit/44ac704fc2d8a2efae427d0cb338c274d82cd128))
* lint the contract, refuse breaking changes to it, and check gen/ is current ([c6ddb87](https://github.com/stupside/castor/commit/c6ddb8730bbe1208acdb1330b7ce830081b30ca0))
* lint the sealed tiers, keep castor-api cgo-free, and release the three binaries ([a48242a](https://github.com/stupside/castor/commit/a48242a66e2bf1c0ecfb0d0862d1173d190af93b))
* **release:** publish only the castor binary ([7b3858b](https://github.com/stupside/castor/commit/7b3858b22f29689b2d698d38b784afac2c3bed16))
* run go fix -diff as the gate itself, so a failure shows its diff ([c2b8014](https://github.com/stupside/castor/commit/c2b8014cc7178d1c48d2fcdbdc4a99ebf6d84e45))
* run once per PR, with -race, and a valid cask stanza ([3807432](https://github.com/stupside/castor/commit/38074321c8abeb786eefc9d1dc23b8317332be7a))

## [1.9.0](https://github.com/stupside/castor/compare/v1.8.1...v1.9.0) (2026-09-22)


### Features

* **ffmpeg:** read a demuxed program as two inputs ([2333d0f](https://github.com/stupside/castor/commit/2333d0f3f027928be826115649fb7151e463e034))
* **media:** let one program span two renditions ([279407f](https://github.com/stupside/castor/commit/279407f795dd13f7a801207cf111e17bd60fe846))
* **release:** ship windows builds, and carry ffmpeg's side feeds over loopback ([#66](https://github.com/stupside/castor/issues/66)) ([5ffeb79](https://github.com/stupside/castor/commit/5ffeb7936199acba403feab2f2a411b32d650edf)), closes [#61](https://github.com/stupside/castor/issues/61)
* **resolve:** keep the chosen variant's audio rendition ([a70b814](https://github.com/stupside/castor/commit/a70b814c9e2300a3b95c7179000565c291682470))


### Bug Fixes

* **cast:** serve sources that need request headers ([#54](https://github.com/stupside/castor/issues/54)) ([f2fe1e1](https://github.com/stupside/castor/commit/f2fe1e11624150052b0d5cc0dad21c60ab9bde1c))
* **deps:** bump golang.org/x/mod v0.38.0 → v0.40.0 ([#62](https://github.com/stupside/castor/issues/62)) ([2cf0627](https://github.com/stupside/castor/commit/2cf0627f2e84bc7306217de82f2b212d09edcf3f))
* **release:** clear quarantine through the install steps homebrew now expects ([#65](https://github.com/stupside/castor/issues/65)) ([9a9b340](https://github.com/stupside/castor/commit/9a9b3408b13e7ce61b0c128702b892d622f1e8e9)), closes [#63](https://github.com/stupside/castor/issues/63)
* **resolve:** never cast a variant that carries no video ([6bb905e](https://github.com/stupside/castor/commit/6bb905e02997a163408763d85e89cf35c9103db1))


### Refactors

* **resolve:** decode HLS playlists with a spec parser ([e714185](https://github.com/stupside/castor/commit/e714185aaa29a6f7242c6e73d44d80ae5c19dfa8))

## [1.8.1](https://github.com/stupside/castor/compare/v1.8.0...v1.8.1) (2026-07-27)


### Bug Fixes

* **ffmpeg:** pass -nostats to the puller invocation ([5fb1650](https://github.com/stupside/castor/commit/5fb165033857fa7e15033150e952f31cbd233723))
* **resolve:** tiebreak equal-bandwidth candidates by height ([3a25c70](https://github.com/stupside/castor/commit/3a25c70173ec67c143e427a6fe72d6e43327e222))

## [1.8.0](https://github.com/stupside/castor/compare/v1.7.1...v1.8.0) (2026-07-27)


### Features

* add Roku cast target ([#50](https://github.com/stupside/castor/issues/50)) ([f109d47](https://github.com/stupside/castor/commit/f109d47c061ea9a2fe2bff31ab8885967fecfde9))
* **cast:** surround audio and compiler-isolated device strategies ([6434ba6](https://github.com/stupside/castor/commit/6434ba659b2cfb77e0003194dd129a83c20c77d8))
* **device:** connect by pinned host, skipping discovery ([dd876cd](https://github.com/stupside/castor/commit/dd876cde770c5501128d2b5b723cb79b6e1bd142)), closes [#24](https://github.com/stupside/castor/issues/24)
* **extract:** disable site isolation to capture cross-origin iframe requests ([bd32c0e](https://github.com/stupside/castor/commit/bd32c0e1d14257cda5aa6cd2d8e6f23aadb62901))


### Bug Fixes

* **cmd:** propagate picked device's type and host, not just name ([3af67b9](https://github.com/stupside/castor/commit/3af67b90e246f018ca424cf8a828d1c19cc90ace))
* **device:** derive each family's SelfFetch from its own selfFetches() ([857ac35](https://github.com/stupside/castor/commit/857ac354d6b92e3d6594da05bb946bd3fc13f0b8))
* **device:** retry DLNA SetAVTransportURI/Play through transient 705 Transport is locked ([6130364](https://github.com/stupside/castor/commit/61303645ae996b1148a60736ba542fc822c26566))
* **ffmpeg:** reject subtitle burn-in without a video encoder ([faf9e25](https://github.com/stupside/castor/commit/faf9e25f7f9d4567bed313f94c549d431b43a11d))
* **media:** normalize BitDepths nil-vs-empty handling to match Profiles ([42dde0b](https://github.com/stupside/castor/commit/42dde0bc812b449e3d9ddbdf199b1ee24c9d0674))


### Refactors

* **cast:** add SelfFetch renderer capability ([d9f9213](https://github.com/stupside/castor/commit/d9f92134e1787a9b630c5ab8eb5c062d0e492410))
* **cast:** capability-driven composition engine ([a7b3f07](https://github.com/stupside/castor/commit/a7b3f07fba7577dd599e737dd52f8ab74d4243fa))
* **cast:** tier renderers below shared building blocks ([2ff4fa8](https://github.com/stupside/castor/commit/2ff4fa8824cdc20c377a1a723eb7c187255b9b6d))
* **device:** dispatch renderer families through a strategy registry ([69d3798](https://github.com/stupside/castor/commit/69d37983f91dd352a030c29ca57c9c78d8c29fd1))
* type sentinel strings as named constants and enums ([b84a396](https://github.com/stupside/castor/commit/b84a3964427bac319bea3e0105a1c4d01b6d3522))


### Documentation

* document how to verify the image SBOM and provenance ([c675665](https://github.com/stupside/castor/commit/c6756652e48078192aeec1a02b088dea9e625fd6))
* document pinning a device by host ([1861a60](https://github.com/stupside/castor/commit/1861a60507f2ad495d704b0b9b3c0c67767fd78b))
* **media:** correct ProbeInfo's blanket unknown-value doc ([eaaae7c](https://github.com/stupside/castor/commit/eaaae7cfaaa8e3a4109ed92c76bf144ef71a3a87))


### Build System

* **docker:** attach an SPDX SBOM and SLSA provenance to the image ([aaaf0ee](https://github.com/stupside/castor/commit/aaaf0ee26c520340b6347011c98f7efde79713e2))
* **docker:** build image with docker bake ([cdb9de6](https://github.com/stupside/castor/commit/cdb9de6338cd787e5e8cd80e2bde43ed7076310b))

## [1.7.1](https://github.com/stupside/castor/compare/v1.7.0...v1.7.1) (2026-07-22)


### Bug Fixes

* **docker:** hw capable ffmpeg with good flag support ([#43](https://github.com/stupside/castor/issues/43)) ([44460a9](https://github.com/stupside/castor/commit/44460a9768fff628996906a521565ed2b872bd69))


### Documentation

* add Trendshift badge ([016a64a](https://github.com/stupside/castor/commit/016a64afabcd34dc7c9420050d77aec17192ad53))
* restructure installation, configuration, and docker sections ([8ecabb2](https://github.com/stupside/castor/commit/8ecabb22112cbc0dd670277e8e621f7a973cef24))

## [1.7.0](https://github.com/stupside/castor/compare/v1.6.2...v1.7.0) (2026-07-21)


### Features

* show cast target device in browse header ([986b3ee](https://github.com/stupside/castor/commit/986b3eef5b4968100676589d4cb6773ef76e93ae))


### Bug Fixes

* **cast:** return error from BuildPlan instead of panicking for unknown device type ([b4c9a6b](https://github.com/stupside/castor/commit/b4c9a6b43e4dfa6be0d8a1250968a7d33bf288a2))
* **cmd:** use CLI framework for --debug flag instead of scanning os.Args ([d4c307b](https://github.com/stupside/castor/commit/d4c307b4ce40f6ffe37ea971e18ab3ae4d66f625))
* config yaml should be optional ([#38](https://github.com/stupside/castor/issues/38)) ([33eea9f](https://github.com/stupside/castor/commit/33eea9faa9e3ab8d146210a9f174e6918b73dc1b))
* **docker:** cli cannot run in castor because of glibc version ([#40](https://github.com/stupside/castor/issues/40)) ([18b6a88](https://github.com/stupside/castor/commit/18b6a88a6a59b5d3ffe9ab3f6947a50ea6dfa82e))
* suppress unchecked Close() lint warnings ([88be120](https://github.com/stupside/castor/commit/88be1209f3569d5bd10eeb3b7962786c11ff6a90))
* wire picked device name into config before browse ([c2fa73f](https://github.com/stupside/castor/commit/c2fa73fd4464eca37bf63ac66a324989261e84ab))


### Refactors

* **cast:** collapse deviceConnector and cueSource single-implementation interfaces ([a9f92dd](https://github.com/stupside/castor/commit/a9f92dd103ad4f3c76c3550d8b912e79c9e32f11))
* **media:** simplify FormatForContentType to return (FormatInfo, bool) ([521205c](https://github.com/stupside/castor/commit/521205cef3b5dbf8d24440ddd39b0313e9487cbb))
* remove subtitle font customization support ([d78d5ed](https://github.com/stupside/castor/commit/d78d5ed0a5f43672a410f95023d0679b824f5539))
* **source:** deduplicate MIME tables and unexport Extractor.Extract ([5858b52](https://github.com/stupside/castor/commit/5858b5260884a906ba2eff184fcb2aa11a1c9852))
* **tmdb:** remove dead Page.HasMore method and SearchResult.GenreIDs field ([42c419d](https://github.com/stupside/castor/commit/42c419dc118df0a7ec4a0acd028f074dbe6e00e7))
* **whisper:** collapse WordSink interface and unexport EnsureModel/EnsureVADModel ([142e2ec](https://github.com/stupside/castor/commit/142e2ec53a3bbb5a1f9bf107c8efba38e21f1b14))


### Documentation

* **browse:** remove stale comment on inspector.load ([bebb2b2](https://github.com/stupside/castor/commit/bebb2b28b1509f8a1dad9295c2cb378a8e7853f1))

## [1.6.2](https://github.com/stupside/castor/compare/v1.6.1...v1.6.2) (2026-07-20)


### Bug Fixes

* drop component prefix and use v in release tags ([8c6a853](https://github.com/stupside/castor/commit/8c6a85383c8da1f3fed4a02cb725f73b62277a08))
* remove v prefix from cask download URL ([62c7703](https://github.com/stupside/castor/commit/62c770360ff4a7c7429ec3fc9cb65a0ea1fecd75))


### Documentation

* document resolver max_height option ([5952564](https://github.com/stupside/castor/commit/59525649ec6e47218997317ed9a0f42882b8d977))


### Continuous Integration

* skip push CI on main ([cfec78c](https://github.com/stupside/castor/commit/cfec78c88f85a0429cbccebdbc59448ebdbb4098))

## [1.6.1](https://github.com/stupside/castor/compare/castor-1.6.0...castor-1.6.1) (2026-07-20)


### Bug Fixes

* **dlna:** drive AVTransport and ConnectionManager v1, v2 and v3 ([#23](https://github.com/stupside/castor/issues/23)) ([b18f045](https://github.com/stupside/castor/commit/b18f0451c31e83e8c168190f91eb17a3eb64ed9b))
* pass ggml include path to cmake for Metal .m files ([4b70efd](https://github.com/stupside/castor/commit/4b70efd838113af32b9634acc3d96a8a6039f661))


### Continuous Integration

* fix empty release version and release on ci commits ([a241612](https://github.com/stupside/castor/commit/a241612fe21fcd4e1039e3a3500fe8c89ca26484))

## [1.6.0](https://github.com/stupside/castor/compare/castor-v1.5.0...castor-1.6.0) (2026-07-20)


### Features

* live-edge pacing at realtime with no burst ([4feef28](https://github.com/stupside/castor/commit/4feef282befbe8cebe5a96e343d4a5a431fdfdec))


### Bug Fixes

* reconnect on HTTP 429 with backoff ([a2e6eb5](https://github.com/stupside/castor/commit/a2e6eb5f78bb434f94acc64d2c0b481d6accba5e))
* remove non-canonical timestamp gate from LA-2 ([0b789d4](https://github.com/stupside/castor/commit/0b789d49341cf301dd2fe33fc64b2f608aa60248))


### Refactors

* split HLS fetch from parse ([d1f44dd](https://github.com/stupside/castor/commit/d1f44dd2a5ee940fc2c033ec163e2c4da6989381))

## [1.5.0](https://github.com/stupside/castor/compare/castor-v1.4.3...castor-v1.5.0) (2026-07-20)


### Features

* add badges to the readme ([cf33c6d](https://github.com/stupside/castor/commit/cf33c6dc631297bd3e9a75af9eb3e2907c1da00c))
* add better feedbacks ([cb5b4e3](https://github.com/stupside/castor/commit/cb5b4e3361dac6ab36766b9b423984cd2bc805bb))
* **browse:** genre discovery, rich metadata, and componentized TUI ([898dcdd](https://github.com/stupside/castor/commit/898dcdd45f4520eaf1551c8fd5ff66174388cbca))
* **browse:** tmdb browse tui ([abe7305](https://github.com/stupside/castor/commit/abe73054e6567810001b9d4e077d572c70380cc9))
* **cast:** auto-detect the local interface from the default route ([d36085d](https://github.com/stupside/castor/commit/d36085d825a7f212f8b8e480f6d8e515f9784052))
* **cast:** read-once spooled pipeline with staged execution ([d11493b](https://github.com/stupside/castor/commit/d11493b405cd9bc78d62ff5714bdda25e559ad53))
* **cmd:** load config lazily so scan and info need none ([106afcb](https://github.com/stupside/castor/commit/106afcbc65f836fe142ea8c8fa0047798394624c))
* **config:** default every setting except device and sources ([b544edc](https://github.com/stupside/castor/commit/b544edcae983cc7e13039127e29985312ec3b449))
* discover chromecast devices via mDNS ([20993bc](https://github.com/stupside/castor/commit/20993bc80210514a363dfb1f19703ef631eb49a8))
* discover Chromecast devices via mDNS ([e757f7a](https://github.com/stupside/castor/commit/e757f7aae7913a76d20e8a3012f5760db3f4e389))
* dive into iframe to trigger loading video ([eabc76f](https://github.com/stupside/castor/commit/eabc76f219977fa2158e8bdf05ef150a2acb5954))
* don't use ring buffer anymore ([172f1dc](https://github.com/stupside/castor/commit/172f1dcf81b223d57ed4e557cb41839313dbddd8))
* drop short streams when ranking candidates ([dd93e4d](https://github.com/stupside/castor/commit/dd93e4d79cb1ba75d261b520175249e3e13a4d52))
* first commit ([849910a](https://github.com/stupside/castor/commit/849910acaf53265206dfb7d8ce55ae92ffe80da5))
* make logs a little bit better looking ([4bfa393](https://github.com/stupside/castor/commit/4bfa39300f2ac05981bc61ef810ffb3143f052ba))
* **release:** static CGO whisper.cpp via matrix + zig cross-compilation ([48feee9](https://github.com/stupside/castor/commit/48feee98c2c2f88d1b68146b81ea656e5276117f))
* replay real browser headers to ffmpeg and ffprobe ([7ef788f](https://github.com/stupside/castor/commit/7ef788f06d4f35264d4ce99c696bf11cf11fbb56))
* simplify browse tui access ([7b13c18](https://github.com/stupside/castor/commit/7b13c18d830fc63c31ab7720589ab2588c39a26a))
* **tmdb:** add genre, discover, and details endpoints ([3bac0d5](https://github.com/stupside/castor/commit/3bac0d58bdb1bf82475988610940201a792cbc00))
* update docker run instruction with working proxy ([cf5e010](https://github.com/stupside/castor/commit/cf5e010c094690d6531a1534d144094dbfbcd976))
* **whisper:** in-process transcription via whisper.cpp ([a09d67d](https://github.com/stupside/castor/commit/a09d67df125034414c74d4544452c36e3156691a))
* **whisper:** stream subtitles via LocalAgreement-2, VAD, and a realtime-paced encoder ([1386dec](https://github.com/stupside/castor/commit/1386dec6d97f7cefda50571ad2c55ce2c6574f2d))


### Bug Fixes

* apply HLS-only ffmpeg input flags to HLS sources only ([60207bc](https://github.com/stupside/castor/commit/60207bc6e8a8cbf8751844fa799e42407985b264))
* clear quarantine xattr in cask postflight ([1d15a29](https://github.com/stupside/castor/commit/1d15a2921e729eecbf2d18beaeba5d1a18f7da07))
* clear quarantine xattr in cask postflight so castor runs after brew install ([c425683](https://github.com/stupside/castor/commit/c425683143f633e7de94d1406fd3328302fc543c)), closes [#17](https://github.com/stupside/castor/issues/17)
* **config:** keep defaults when a section is present but empty ([bc9fd8b](https://github.com/stupside/castor/commit/bc9fd8b02ac438f293bfbc4e4c72705390824e36))
* **dlna:** stop pacing delivery to the renderer ([81183ee](https://github.com/stupside/castor/commit/81183ee383eb342899419cc7bbf7434ab6fa3baa))
* docker image has old ffmpeg version ([0affafa](https://github.com/stupside/castor/commit/0affafa4d39ff3bc0fda9b954a0b77693230dbae))
* **docker:** install the ffmpeg/chromium/TLS runtime the pipeline needs ([bd1cb14](https://github.com/stupside/castor/commit/bd1cb14ae2a3119f88822e47ad610c7b2685c96e))
* **extract:** pass --disable-dev-shm-usage to chromium ([a793431](https://github.com/stupside/castor/commit/a79343150288396fb18723679cec9620aa77e6b1))
* **extract:** reap headless Chrome on session teardown ([aa56480](https://github.com/stupside/castor/commit/aa5648077a1546b903692ae796d2e68c5a4822a3))
* let real request headers win over header-less captures ([b9f6632](https://github.com/stupside/castor/commit/b9f6632b34e31bcc58f3831d1a16cddc36969025))
* **release:** build whisper with GGML_NATIVE=OFF for portable binaries ([98efaa8](https://github.com/stupside/castor/commit/98efaa8b0ac6c87abcebe53152a7b4d543f79a82))
* **release:** ignore .zig-cache and whisper build_* dirs ([d58ee28](https://github.com/stupside/castor/commit/d58ee28e5a4bec692a4ebabb7d756eb0b6acc6a3))
* **release:** matrix parallel whisper builds; stub install_name_tool for darwin cross ([114775c](https://github.com/stupside/castor/commit/114775c943d308511454189153714541ac20a3cd))
* **release:** native runners for whisper builds, no cross-compile hacks ([2c0b780](https://github.com/stupside/castor/commit/2c0b78037999b09cdf2d37a1ba6d6d88c307f5fc))
* **release:** replace Pro-only split/merge with single-runner zig cross-compilation ([976eab6](https://github.com/stupside/castor/commit/976eab61e302bb79bfd574565afbba1f308cf227))
* **release:** use MAJOR.MINOR.PATCH format for zig macOS target triple ([6ca20fd](https://github.com/stupside/castor/commit/6ca20fd530c83ae3986a7781982d0a4c8d1b86c3))
* **resolve:** drop decoy streams with no castable video+audio ([4d0f14d](https://github.com/stupside/castor/commit/4d0f14de0b6aaea442224a3106af89f4d4fd3642))
* send browser request headers to puller so hotlinked streams work ([5651dd9](https://github.com/stupside/castor/commit/5651dd9b0747d947d615d1eb194bfc7477598a12))
* send browser request headers to puller so hotlinked streams work ([ca50081](https://github.com/stupside/castor/commit/ca50081758673da2b4262c11069eb5128520fcf3)), closes [#14](https://github.com/stupside/castor/issues/14)
* stream buffers too much ([eeb5bb9](https://github.com/stupside/castor/commit/eeb5bb995308d3838b5294d520578a0e788a39b7))
* stream can stop after some time ([e1aef10](https://github.com/stupside/castor/commit/e1aef10029e24f5fe276139e0fcda3914cbced3e))


### Refactors

* **cast:** split cue shaping out of whisper into a cue package ([1e2ea3c](https://github.com/stupside/castor/commit/1e2ea3c7ee53c064452223835ba26781f44f5572))
* **cmd:** typed config wiring ([a5fcc76](https://github.com/stupside/castor/commit/a5fcc761f6f26535048e5caa7a067c8efa73ade1))
* **config:** compose per-package configs ([067977b](https://github.com/stupside/castor/commit/067977b2bc235ded0011f9864265570e8278532d))
* **device:** flatten renderers behind a connect factory ([4c02e50](https://github.com/stupside/castor/commit/4c02e50085e37e577fdbd23b519b3cdb73c0f2a2))
* make sources an array without names, remove --source flag ([657d041](https://github.com/stupside/castor/commit/657d0414d8619b267331ab80da168af71f48a933))
* **media:** add http header helpers ([6360bf9](https://github.com/stupside/castor/commit/6360bf9726e54594ff2c8ef0a432446a6967d7e8))
* mirror DLNA discovery on the chromecast pattern ([afa52f1](https://github.com/stupside/castor/commit/afa52f1f31e3a1b667786d97c81e3360928d3964))
* modernize Discover and gate device interface impls ([b277fef](https://github.com/stupside/castor/commit/b277fefb2df9be2d52604fbf8c0ddb38d97aa326))
* **replay:** remove the now-unused token bucket ([7858d0e](https://github.com/stupside/castor/commit/7858d0eaa0fecede13e122e76e3760c7a274fb8a))
* **source:** group extraction and resolution under internal/source ([c0eeee4](https://github.com/stupside/castor/commit/c0eeee402cc3980e7c2810177c96adbcdbc3c38a))
* use explicit 2xx range check instead of the /100 trick ([3999cab](https://github.com/stupside/castor/commit/3999cab68015a21bb5229805d68a95fd54bcec91))


### Documentation

* add a castor mascot to the README ([be9cd9b](https://github.com/stupside/castor/commit/be9cd9b9b67ae3e61940306927d869badb7345b1))
* document Docker usage ([ab0dfbd](https://github.com/stupside/castor/commit/ab0dfbda1794f35746c405400c84b3781d2fce75))
* document subtitle generation and source build ([b90c621](https://github.com/stupside/castor/commit/b90c62114d7ab7eca314e8b511818a7aad954897))
* drop stale references to the send pacer ([8157dd9](https://github.com/stupside/castor/commit/8157dd9071cb3f7a01a2d51d2d4f939907f35ffd))
* minimal config and direnv setup ([f925ca9](https://github.com/stupside/castor/commit/f925ca9584891fa57c2f00ce387f9dd0e62fb1bf))
* overhaul README, add CONTRIBUTING and SECURITY ([e010f18](https://github.com/stupside/castor/commit/e010f181ba2742dd5349910dfe05ed0de8522bd5))
* **readme:** add Installation section (Homebrew, Docker, source) ([a1c5d13](https://github.com/stupside/castor/commit/a1c5d1399d36a070ab1e43652fbf0cac38540148))
* **readme:** fix stale commands, add config quickstart and screenshots ([b01c55e](https://github.com/stupside/castor/commit/b01c55edc1a5a2428ffe5a9c93be0ff30e9f3ff9))
