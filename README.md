# kmeans

* Uses `GHC 9.0.2`

* Run to build
    ```sh
    $ stack build
    ```

* HLS logs
    ```sh
    $ ghcup run haskell-language-server-wrapper

    [ Info  ] downloading: https://raw.githubusercontent.com/haskell/ghcup-metadata/master/ghcup-0.0.7.yaml as file /home/user/.ghcup/cache/ghcup-0.0.7.yaml
    % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                    Dload  Upload   Total   Spent    Left  Speed
    0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
    [ Warn  ] New ghc version available. To upgrade, run 'ghcup install ghc 9.2.4'
    Found "/home/user/Desktop/kmeans/hie.yaml" for "/home/user/Desktop/kmeans/a"
    Run entered for haskell-language-server-wrapper(haskell-language-server-wrapper) Version 1.7.0.0 x86_64 ghc-9.2.2
    Current directory: /home/user/Desktop/kmeans
    Operating system: linux
    Arguments: []
    Cradle directory: /home/user/Desktop/kmeans
    Cradle type: Stack

    Tool versions found on the $PATH
    cabal:          3.6.2.0
    stack:          2.7.5
    ghc:            9.0.2


    Consulting the cradle to get project GHC version...
    Project GHC version: 9.0.2
    haskell-language-server exe candidates: ["haskell-language-server-9.0.2","haskell-language-server"]
    Launching haskell-language-server exe at:/home/user/.ghcup/bin/haskell-language-server-9.0.2
    2022-08-03T08:10:52.000559Z | Info | No log file specified; using stderr.
    2022-08-03T08:10:52.000980Z | Info | haskell-language-server version: 1.7.0.0 (GHC: 9.0.2) (PATH: /home/user/.ghcup/hls/1.7.0.0/lib/haskell-language-server-1.7.0.0/bin/haskell-language-server-9.0.2)
    2022-08-03T08:10:52.001666Z | Info | Directory: /home/user/Desktop/kmeans
    2022-08-03T08:10:52.001980Z | Info | Logging heap statistics every 60.00s
    ghcide setup tester in /home/user/Desktop/kmeans.
    Report bugs at https://github.com/haskell/haskell-language-server/issues

    Step 1/4: Finding files to test in /home/user/Desktop/kmeans
    Found 2 files

    Step 2/4: Looking for hie.yaml files that control setup
    Found 1 cradle
    (/home/user/Desktop/kmeans/hie.yaml)

    Step 3/4: Initializing the IDE

    Step 4/4: Type checking the files
    2022-08-03T08:10:52.009420Z | Info | Cradle path: my-kmeans/kmeans.hs
    2022-08-03 13:10:52.348555618 [ThreadId 36] INFO hie-bios:      Using main module: 1. Package `kmeans' component kmeans:exe:my-kmeans-exe with main-is file: /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    2022-08-03 13:10:52.47323547 [ThreadId 36] INFO hie-bios:       Building all executables for `kmeans' once. After a successful build of all of them, only specified executables will be rebuilt.
    2022-08-03 13:10:52.495197654 [ThreadId 36] INFO hie-bios:      kmeans> configure (exe)
    2022-08-03 13:10:52.867147109 [ThreadId 36] INFO hie-bios:      Configuring kmeans-0.1.0.0...
    2022-08-03 13:10:53.106060303 [ThreadId 36] INFO hie-bios:      kmeans> initial-build-steps (exe)
    2022-08-03 13:10:53.246452462 [ThreadId 36] INFO hie-bios:      The following GHC options are incompatible with GHCi and have not been passed to it: -threaded
    2022-08-03 13:10:53.246562644 [ThreadId 36] INFO hie-bios:      Configuring GHCi with the following packages: kmeans
    2022-08-03 13:10:53.731899227 [ThreadId 43] INFO hie-bios:      /home/user/Desktop/kmeans/.stack-work/install/x86_64-linux-tinfo6/32e43fc6f72454bd9c6d5584522641d944ec81fc26e595aa3e0ee2a243113912/9.0.2/pkgdb:/home/user/.stack/snapshots/x86_64-linux-tinfo6/32e43fc6f72454bd9c6d5584522641d944ec81fc26e595aa3e0ee2a243113912/9.0.2/pkgdb:/home/user/.stack/programs/x86_64-linux/ghc-tinfo6-9.0.2/lib/ghc-9.0.2/package.conf.d
    2022-08-03T08:10:54.822300Z | Info | Interface files cache directory: /home/user/.cache/ghcide/main-5961337d92f408a08eaefecd5b95b54550481845
    2022-08-03T08:10:54.822696Z | Info | Making new HscEnv. In-place unit ids: [main]
    2022-08-03T08:10:55.131764Z | Info | updateFileDiagnostics published different from new diagnostics - file diagnostics: File:     /home/user/Desktop/kmeans/my-kmeans/KMeansCore.hs
    Hidden:   no
    Range:    5:1-5:36
    Source:   hlint
    Severity: DsInfo
    Message:  Unused LANGUAGE pragmaFound:{-# LANGUAGE DeriveDataTypeable #-}Why not:
    File:     /home/user/Desktop/kmeans/my-kmeans/KMeansCore.hs
    Hidden:   no
    Range:    36:9-36:50
    Source:   hlint
    Severity: DsInfo
    Message:  Use <$>Found:do a <- getb <- getreturn (Point a b)Why not:do a <- getPoint a <$> get
    2022-08-03T08:10:55.241678Z | Info | updateFileDiagnostics published different from new diagnostics - file diagnostics: File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    1:1-1:51
    Source:   hlint
    Severity: DsInfo
    Message: 
    Unused LANGUAGE pragma
    Found:
    {-# LANGUAGE ScopedTypeVariables, BangPatterns #-}
    Why not:
    {-# LANGUAGE ScopedTypeVariables #-}
    Extension BangPatterns is not used
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    76:1-76:58
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_seq :: Int -> [Point] -> [Cluster] -> IO [Cluster]
    Why not:
    kmeansSeq :: Int -> [Point] -> [Cluster] -> IO [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    77:1-91:18
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_seq nclusters points clusters = ...
    Why not:
    kmeansSeq nclusters points clusters = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    100:1-100:67
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_strat :: Int -> Int -> [Point] -> [Cluster] -> IO [Cluster]
    Why not:
    kmeansStrat :: Int -> Int -> [Point] -> [Cluster] -> IO [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    101:1-117:18
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_strat numChunks nclusters points clusters = ...
    Why not:
    kmeansStrat numChunks nclusters points clusters = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    133:1-133:65
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_par :: Int -> Int -> [Point] -> [Cluster] -> IO [Cluster]
    Why not:
    kmeansPar :: Int -> Int -> [Point] -> [Cluster] -> IO [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    134:1-150:18
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_par mappers nclusters points clusters = ...
    Why not:
    kmeansPar mappers nclusters points clusters = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    155:1-155:76
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_div_par ::
    Int -> Int -> [Point] -> [Cluster] -> Int -> IO [Cluster]
    Why not:
    kmeansDivPar ::
    Int -> Int -> [Point] -> [Cluster] -> Int -> IO [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    156:1-181:18
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_div_par threshold nclusters points clusters npoints = ...
    Why not:
    kmeansDivPar threshold nclusters points clusters npoints = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    201:1-201:77
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_div_eval ::
    Int -> Int -> [Point] -> [Cluster] -> Int -> IO [Cluster]
    Why not:
    kmeansDivEval ::
    Int -> Int -> [Point] -> [Cluster] -> Int -> IO [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    202:1-227:18
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    kmeans_div_eval threshold nclusters points clusters npoints = ...
    Why not:
    kmeansDivEval threshold nclusters points clusters npoints = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    286:1-286:61
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    parSteps_strat :: Int -> [Cluster] -> [[Point]] -> [Cluster]
    Why not:
    parStepsStrat :: Int -> [Cluster] -> [[Point]] -> [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    287:1-291:34
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    parSteps_strat nclusters clusters pointss = ...
    Why not:
    parStepsStrat nclusters clusters pointss = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    289:22-289:23
    Source:   hlint
    Severity: DsInfo
    Message: 
    Redundant $
    Found:
    foldr1 combine
    $ (map (assign nclusters clusters) pointss `using` parList rseq)
    Why not:
    foldr1
    combine
    (map (assign nclusters clusters) pointss `using` parList rseq)
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    294:1-294:56
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    steps_par :: Int -> [Cluster] -> [[Point]] -> [Cluster]
    Why not:
    stepsPar :: Int -> [Cluster] -> [[Point]] -> [Cluster]
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    295:1-298:68
    Source:   hlint
    Severity: DsInfo
    Message: 
    Use camelCase
    Found:
    steps_par nclusters clusters pointss = ...
    Why not:
    stepsPar nclusters clusters pointss = ...
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    297:7-298:68
    Source:   hlint
    Severity: DsInfo
    Message: 
    Move brackets to avoid $
    Found:
    foldl1' combine
    $ (runPar $ Par.parMap (assign nclusters clusters) pointss)
    Why not:
    foldl1' combine
    $ runPar (Par.parMap (assign nclusters clusters) pointss)
    File:     /home/user/Desktop/kmeans/my-kmeans/kmeans.hs
    Hidden:   no
    Range:    297:23-297:24
    Source:   hlint
    Severity: DsInfo
    Message: 
    Redundant $
    Found:
    foldl1' combine
    $ (runPar $ Par.parMap (assign nclusters clusters) pointss)
    Why not:
    foldl1'
    combine (runPar $ Par.parMap (assign nclusters clusters) pointss)
    2022-08-03T08:10:55.277236Z | Info | updateFileDiagnostics published different from new diagnostics - file diagnostics: File:     /home/user/Desktop/kmeans/my-kmeans/KMeansCore.hs
    Hidden:   no
    Range:    5:1-5:36
    Source:   hlint
    Severity: DsInfo
    Message:  Unused LANGUAGE pragmaFound:{-# LANGUAGE DeriveDataTypeable #-}Why not:
    File:     /home/user/Desktop/kmeans/my-kmeans/KMeansCore.hs
    Hidden:   no
    Range:    36:9-36:50
    Source:   hlint
    Severity: DsInfo
    Message:  Use <$>Found:do a <- getb <- getreturn (Point a b)Why not:do a <- getPoint a <$> get
    ```
    and
    ```
    File:     /home/user/Desktop/kmeans/my-kmeans/KMeansCore.hs
    Hidden:   no
    Range:    1:1-2:1
    Source:   typecheck
    Severity: DsError
    Message: 
    Unexpected usage error
    /home/user/.stack/snapshots/x86_64-linux-tinfo6/9c48492b149e18ce129fd00f656e45a2602c4cb44a4c4d2fb6ca174960b4277a/9.0.2/lib/x86_64-linux-ghc-9.0.2/libHSprimitive-0.7.3.0-EikPDi9CXNiB9f5MDJybeY-ghc9.0.2.so:
    undefined symbol: base_GHCziRead_list3_info
    Files that failed:
    * /home/user/Desktop/kmeans/my-kmeans/KMeansCore.hs
    * /home/user/Desktop/kmeans/my-kmeans/kmeans.hs

    Completed (0 files worked, 2 files failed)
    ```