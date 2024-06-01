# Comparing `tmp/ampel_hu_astro-0.8.4a2.tar.gz` & `tmp/ampel_hu_astro-0.8.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_hu_astro-0.8.4a2.tar", max compression
+gzip compressed data, was "ampel_hu_astro-0.8.4a3.tar", max compression
```

## Comparing `ampel_hu_astro-0.8.4a2.tar` & `ampel_hu_astro-0.8.4a3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     1512 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/LICENSE
--rw-r--r--   0        0        0     9363 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/README.md
--rw-r--r--   0        0        0     3122 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py
--rw-r--r--   0        0        0     8895 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py
--rw-r--r--   0        0        0     3592 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/ResourceDependentConsumer.py
--rwxr-xr-x   0        0        0     1461 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py
--rw-r--r--   0        0        0     1970 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/channel_notes.txt
--rwxr-xr-x   0        0        0     2185 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py
--rw-r--r--   0        0        0        0 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/py.typed
--rwxr-xr-x   0        0        0      981 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/LensedTransientFilter.py
--rw-r--r--   0        0        0     2066 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/PredetectionFilter.py
--rw-r--r--   0        0        0      732 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/RandFilter.py
--rwxr-xr-x   0        0        0    15789 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/RcfFilter.py
--rw-r--r--   0        0        0     6142 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
--rwxr-xr-x   0        0        0    10713 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/SimpleDecentFilter.py
--rwxr-xr-x   0        0        0    11644 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/StellarFilter.py
--rwxr-xr-x   0        0        0     3844 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/TransientInClusterFilter.py
--rwxr-xr-x   0        0        0     4843 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/XShooterFilter.py
--rw-r--r--   0        0        0     6941 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2BaseLightcurveFitter.py
--rw-r--r--   0        0        0    59244 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2BayesianBlocks.py
--rwxr-xr-x   0        0        0     4932 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2BrightSNProb.py
--rwxr-xr-x   0        0        0    11158 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
--rw-r--r--   0        0        0     2501 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2DemoLightcurveFitter.py
--rw-r--r--   0        0        0    21870 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2DigestRedshifts.py
--rw-r--r--   0        0        0    33145 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2DustEchoEval.py
--rw-r--r--   0        0        0    11549 2024-05-31 07:01:45.119593 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
--rw-r--r--   0        0        0    24754 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2ElasticcReport.py
--rwxr-xr-x   0        0        0     2378 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2FastDecliner.py
--rw-r--r--   0        0        0     8706 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2GetLensSNParameters.py
--rwxr-xr-x   0        0        0     5369 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2HealpixProb.py
--rw-r--r--   0        0        0    15644 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2InfantCatalogEval.py
--rw-r--r--   0        0        0    35779 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2KilonovaEval.py
--rw-r--r--   0        0        0     5824 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2KilonovaStats.py
--rwxr-xr-x   0        0        0    10191 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2LCQuality.py
--rw-r--r--   0        0        0    10357 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2LSPhotoZTap.py
--rw-r--r--   0        0        0     2250 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2LoadRedshift.py
--rw-r--r--   0        0        0     3633 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MatchBTS.py
--rw-r--r--   0        0        0     5353 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MatchGRB.py
--rwxr-xr-x   0        0        0     5277 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MinorPlanetCenter.py
--rw-r--r--   0        0        0     9680 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MultiXgbClassifier.py
--rwxr-xr-x   0        0        0     6607 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2NedSNCosmo.py
--rwxr-xr-x   0        0        0     7132 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2NedTap.py
--rwxr-xr-x   0        0        0     5646 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2Observability.py
--rwxr-xr-x   0        0        0     3364 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
--rwxr-xr-x   0        0        0     5965 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
--rwxr-xr-x   0        0        0     4538 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
--rwxr-xr-x   0        0        0     2831 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py
--rw-r--r--   0        0        0    10489 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PhaseLimit.py
--rw-r--r--   0        0        0     2584 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PolynomialFit.py
--rw-r--r--   0        0        0     1979 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PropagateStockInfo.py
--rwxr-xr-x   0        0        0    15779 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RiseDeclineStat.py
--rw-r--r--   0        0        0    19608 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunParsnip.py
--rw-r--r--   0        0        0    10460 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunPossis.py
--rw-r--r--   0        0        0    21719 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunSncosmo.py
--rw-r--r--   0        0        0    10803 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunSnoopy.py
--rw-r--r--   0        0        0     5941 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunTDE.py
--rw-r--r--   0        0        0      236 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2SNCosmo.py
--rw-r--r--   0        0        0    20992 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2TNSEval.py
--rw-r--r--   0        0        0    26199 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
--rw-r--r--   0        0        0    10470 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2XgbClassifier.py
--rw-r--r--   0        0        0   139314 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json
--rw-r--r--   0        0        0    91172 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json
--rw-r--r--   0        0        0    71112 2024-05-31 07:01:45.123592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json
--rw-r--r--   0        0        0  8028781 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/xgb_trees.py
--rw-r--r--   0        0        0     3254 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/AbsScoreCalculator.py
--rw-r--r--   0        0        0     3980 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/AstroColibriClient.py
--rw-r--r--   0        0        0    12550 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/AstroColibriPublisher.py
--rwxr-xr-x   0        0        0     5598 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
--rw-r--r--   0        0        0     2362 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/CostCounter.py
--rwxr-xr-x   0        0        0    13326 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/DCachePublisher.py
--rw-r--r--   0        0        0    10625 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ElasticcClassPublisher.py
--rw-r--r--   0        0        0     3565 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ElasticcTomClient.py
--rw-r--r--   0        0        0    10057 2024-05-31 07:01:45.143592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/HealpixCorrPlotter.py
--rw-r--r--   0        0        0     7041 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/HealpixTokenGenerator.py
--rw-r--r--   0        0        0    11976 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/PlotLightcurveSample.py
--rwxr-xr-x   0        0        0    18404 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/PlotTransientLightcurves.py
--rw-r--r--   0        0        0     4355 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RandomMapGenerator.py
--rwxr-xr-x   0        0        0     5253 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RapidBase.py
--rwxr-xr-x   0        0        0    12504 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RapidLco.py
--rwxr-xr-x   0        0        0     4008 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RapidSedm.py
--rw-r--r--   0        0        0     1647 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ScoreSingleObject.py
--rw-r--r--   0        0        0     3342 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ScoreTNSObjects.py
--rwxr-xr-x   0        0        0    11948 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/SlackSummaryPublisher.py
--rw-r--r--   0        0        0     7508 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/SubmitTNS.py
--rwxr-xr-x   0        0        0     1957 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TNSMirrorUpdater.py
--rwxr-xr-x   0        0        0     2849 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TransientInfoPrinter.py
--rw-r--r--   0        0        0     9198 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TransientTablePublisher.py
--rwxr-xr-x   0        0        0     4304 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TransientViewDumper.py
--rw-r--r--   0        0        0     5173 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/VOEventPublisher.py
--rwxr-xr-x   0        0        0     2267 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py
--rwxr-xr-x   0        0        0     6500 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSClient.py
--rw-r--r--   0        0        0     4100 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSMirrorDB.py
--rwxr-xr-x   0        0        0     1738 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSName.py
--rw-r--r--   0        0        0      130 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSToken.py
--rw-r--r--   0        0        0      118 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/__init__.py
--rw-r--r--   0        0        0     6133 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/tns_ampel_util.py
--rw-r--r--   0        0        0    20855 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json
--rw-r--r--   0        0        0      634 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_config.py
--rw-r--r--   0        0        0      150 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_flatten.py
--rw-r--r--   0        0        0     4750 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_slackpublisher.py
--rw-r--r--   0        0        0     3350 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_t2brightsnprob.py
--rw-r--r--   0        0        0      468 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_tns.py
--rw-r--r--   0        0        0     8132 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/AmpelHealpix.py
--rw-r--r--   0        0        0     2585 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/automation/get_kn.py
--rw-r--r--   0        0        0     2394 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/automation/jobfileCaller.py
--rw-r--r--   0        0        0     3606 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/automation/jobfileWriter.py
--rw-r--r--   0        0        0      882 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/flatten.py
--rw-r--r--   0        0        0     1043 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/ned.py
--rw-r--r--   0        0        0      408 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/ampel/contrib/hu/utils.py
--rw-r--r--   0        0        0     5328 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/alias.yml
--rw-r--r--   0        0        0     2992 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml
--rw-r--r--   0        0        0     1858 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/channel/HU_STELLAR_OUTBURST.yml
--rw-r--r--   0        0        0      992 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/ChannelSummary.yml
--rw-r--r--   0        0        0      982 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/RapidReact.yml
--rw-r--r--   0        0        0      801 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/StellarPost.yml
--rw-r--r--   0        0        0      205 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/UpdateTNSMirror.yml
--rw-r--r--   0        0        0     2895 2024-05-31 07:01:45.147592 ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/unit.yml
--rw-r--r--   0        0        0     5208 2024-05-31 07:01:45.259593 ampel_hu_astro-0.8.4a2/pyproject.toml
--rw-r--r--   0        0        0    12245 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.4a2/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/LICENSE
+-rw-r--r--   0        0        0     9363 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/README.md
+-rw-r--r--   0        0        0     3122 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py
+-rw-r--r--   0        0        0     8895 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py
+-rw-r--r--   0        0        0     3592 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/ResourceDependentConsumer.py
+-rwxr-xr-x   0        0        0     1461 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py
+-rw-r--r--   0        0        0     1970 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/channel_notes.txt
+-rwxr-xr-x   0        0        0     2185 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/py.typed
+-rwxr-xr-x   0        0        0      981 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/LensedTransientFilter.py
+-rw-r--r--   0        0        0     2066 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/PredetectionFilter.py
+-rw-r--r--   0        0        0      732 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/RandFilter.py
+-rwxr-xr-x   0        0        0    15789 2024-06-01 18:27:41.526423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/RcfFilter.py
+-rw-r--r--   0        0        0     6142 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
+-rwxr-xr-x   0        0        0    10713 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/SimpleDecentFilter.py
+-rwxr-xr-x   0        0        0    11644 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/StellarFilter.py
+-rwxr-xr-x   0        0        0     3844 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/TransientInClusterFilter.py
+-rwxr-xr-x   0        0        0     4843 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/XShooterFilter.py
+-rw-r--r--   0        0        0     6941 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2BaseLightcurveFitter.py
+-rw-r--r--   0        0        0    59244 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2BayesianBlocks.py
+-rwxr-xr-x   0        0        0     4932 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2BrightSNProb.py
+-rwxr-xr-x   0        0        0    11158 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
+-rw-r--r--   0        0        0     2501 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2DemoLightcurveFitter.py
+-rw-r--r--   0        0        0    21870 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2DigestRedshifts.py
+-rw-r--r--   0        0        0    33145 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2DustEchoEval.py
+-rw-r--r--   0        0        0    11549 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
+-rw-r--r--   0        0        0    24754 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2ElasticcReport.py
+-rwxr-xr-x   0        0        0     2378 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2FastDecliner.py
+-rw-r--r--   0        0        0     8706 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2GetLensSNParameters.py
+-rwxr-xr-x   0        0        0     5369 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2HealpixProb.py
+-rw-r--r--   0        0        0    15644 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2InfantCatalogEval.py
+-rw-r--r--   0        0        0    35779 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2KilonovaEval.py
+-rw-r--r--   0        0        0     5824 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2KilonovaStats.py
+-rwxr-xr-x   0        0        0    10191 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2LCQuality.py
+-rw-r--r--   0        0        0    10357 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2LSPhotoZTap.py
+-rw-r--r--   0        0        0     2250 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2LoadRedshift.py
+-rw-r--r--   0        0        0     3633 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MatchBTS.py
+-rw-r--r--   0        0        0     5353 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MatchGRB.py
+-rwxr-xr-x   0        0        0     5277 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MinorPlanetCenter.py
+-rw-r--r--   0        0        0     9680 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MultiXgbClassifier.py
+-rwxr-xr-x   0        0        0     6607 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2NedSNCosmo.py
+-rwxr-xr-x   0        0        0     7132 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2NedTap.py
+-rwxr-xr-x   0        0        0     5646 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2Observability.py
+-rwxr-xr-x   0        0        0     3364 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
+-rwxr-xr-x   0        0        0     5965 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
+-rwxr-xr-x   0        0        0     4538 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
+-rwxr-xr-x   0        0        0     2831 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py
+-rw-r--r--   0        0        0    10489 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PhaseLimit.py
+-rw-r--r--   0        0        0     2584 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PolynomialFit.py
+-rw-r--r--   0        0        0     1979 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PropagateStockInfo.py
+-rwxr-xr-x   0        0        0    15779 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RiseDeclineStat.py
+-rw-r--r--   0        0        0    19608 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunParsnip.py
+-rw-r--r--   0        0        0    10460 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunPossis.py
+-rw-r--r--   0        0        0    21719 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunSncosmo.py
+-rw-r--r--   0        0        0    10803 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunSnoopy.py
+-rw-r--r--   0        0        0     5941 2024-06-01 18:27:41.530423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunTDE.py
+-rw-r--r--   0        0        0      236 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2SNCosmo.py
+-rw-r--r--   0        0        0    20992 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2TNSEval.py
+-rw-r--r--   0        0        0    26199 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
+-rw-r--r--   0        0        0    10470 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2XgbClassifier.py
+-rw-r--r--   0        0        0   139314 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json
+-rw-r--r--   0        0        0    91172 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json
+-rw-r--r--   0        0        0    71112 2024-06-01 18:27:41.534423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json
+-rw-r--r--   0        0        0  8028781 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/xgb_trees.py
+-rw-r--r--   0        0        0     3254 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/AbsScoreCalculator.py
+-rw-r--r--   0        0        0     3980 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/AstroColibriClient.py
+-rw-r--r--   0        0        0    12550 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/AstroColibriPublisher.py
+-rwxr-xr-x   0        0        0     5598 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
+-rw-r--r--   0        0        0     2362 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/CostCounter.py
+-rwxr-xr-x   0        0        0    13326 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/DCachePublisher.py
+-rw-r--r--   0        0        0    10625 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ElasticcClassPublisher.py
+-rw-r--r--   0        0        0     3565 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ElasticcTomClient.py
+-rw-r--r--   0        0        0    10057 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/HealpixCorrPlotter.py
+-rw-r--r--   0        0        0     7041 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/HealpixTokenGenerator.py
+-rw-r--r--   0        0        0    11976 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/PlotLightcurveSample.py
+-rwxr-xr-x   0        0        0    18399 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/PlotTransientLightcurves.py
+-rw-r--r--   0        0        0     4355 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RandomMapGenerator.py
+-rwxr-xr-x   0        0        0     5253 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RapidBase.py
+-rwxr-xr-x   0        0        0    12504 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RapidLco.py
+-rwxr-xr-x   0        0        0     4008 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RapidSedm.py
+-rw-r--r--   0        0        0     1647 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ScoreSingleObject.py
+-rw-r--r--   0        0        0     3342 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ScoreTNSObjects.py
+-rwxr-xr-x   0        0        0    11948 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/SlackSummaryPublisher.py
+-rw-r--r--   0        0        0     7508 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/SubmitTNS.py
+-rwxr-xr-x   0        0        0     1957 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TNSMirrorUpdater.py
+-rwxr-xr-x   0        0        0     2849 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TransientInfoPrinter.py
+-rw-r--r--   0        0        0     9198 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TransientTablePublisher.py
+-rwxr-xr-x   0        0        0     4304 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TransientViewDumper.py
+-rw-r--r--   0        0        0     5173 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/VOEventPublisher.py
+-rwxr-xr-x   0        0        0     2267 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py
+-rwxr-xr-x   0        0        0     6500 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSClient.py
+-rw-r--r--   0        0        0     4100 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSMirrorDB.py
+-rwxr-xr-x   0        0        0     1738 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSName.py
+-rw-r--r--   0        0        0      130 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSToken.py
+-rw-r--r--   0        0        0      118 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/__init__.py
+-rw-r--r--   0        0        0     6133 2024-06-01 18:27:41.554423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/tns_ampel_util.py
+-rw-r--r--   0        0        0    20855 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json
+-rw-r--r--   0        0        0      634 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_config.py
+-rw-r--r--   0        0        0      150 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_flatten.py
+-rw-r--r--   0        0        0     4750 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_slackpublisher.py
+-rw-r--r--   0        0        0     3350 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_t2brightsnprob.py
+-rw-r--r--   0        0        0      468 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_tns.py
+-rw-r--r--   0        0        0     8132 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/AmpelHealpix.py
+-rw-r--r--   0        0        0     2585 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/automation/get_kn.py
+-rw-r--r--   0        0        0     2394 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/automation/jobfileCaller.py
+-rw-r--r--   0        0        0     3606 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/automation/jobfileWriter.py
+-rw-r--r--   0        0        0      882 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/flatten.py
+-rw-r--r--   0        0        0     1043 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/ned.py
+-rw-r--r--   0        0        0      408 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/ampel/contrib/hu/utils.py
+-rw-r--r--   0        0        0     5328 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/alias.yml
+-rw-r--r--   0        0        0     2992 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml
+-rw-r--r--   0        0        0     1858 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/channel/HU_STELLAR_OUTBURST.yml
+-rw-r--r--   0        0        0      992 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/ChannelSummary.yml
+-rw-r--r--   0        0        0     1021 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/RapidReact.yml
+-rw-r--r--   0        0        0      850 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/StellarPost.yml
+-rw-r--r--   0        0        0      205 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/UpdateTNSMirror.yml
+-rw-r--r--   0        0        0     2895 2024-06-01 18:27:41.558423 ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/unit.yml
+-rw-r--r--   0        0        0     5208 2024-06-01 18:27:41.654422 ampel_hu_astro-0.8.4a3/pyproject.toml
+-rw-r--r--   0        0        0    12245 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.4a3/PKG-INFO
```

### Comparing `ampel_hu_astro-0.8.4a2/LICENSE` & `ampel_hu_astro-0.8.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/README.md` & `ampel_hu_astro-0.8.4a3/README.md`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/ResourceDependentConsumer.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/ResourceDependentConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/channel_notes.txt` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/channel_notes.txt`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/LensedTransientFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/LensedTransientFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/PredetectionFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/PredetectionFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/RandFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/RandFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/RcfFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/RcfFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/RedshiftCatalogFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/RedshiftCatalogFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/SimpleDecentFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/SimpleDecentFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/StellarFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/StellarFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/TransientInClusterFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/TransientInClusterFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t0/XShooterFilter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t0/XShooterFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2BaseLightcurveFitter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2BaseLightcurveFitter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2BayesianBlocks.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2BayesianBlocks.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2BrightSNProb.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2BrightSNProb.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2CatalogMatchLocal.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2CatalogMatchLocal.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2DemoLightcurveFitter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2DemoLightcurveFitter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2DigestRedshifts.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2DigestRedshifts.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2DustEchoEval.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2DustEchoEval.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2ElasticcReport.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2ElasticcReport.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2FastDecliner.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2FastDecliner.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2GetLensSNParameters.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2GetLensSNParameters.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2HealpixProb.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2HealpixProb.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2InfantCatalogEval.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2InfantCatalogEval.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2KilonovaEval.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2KilonovaEval.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2KilonovaStats.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2KilonovaStats.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2LCQuality.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2LCQuality.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2LSPhotoZTap.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2LSPhotoZTap.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2LoadRedshift.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2LoadRedshift.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MatchBTS.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MatchBTS.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MatchGRB.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MatchGRB.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MinorPlanetCenter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MinorPlanetCenter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2MultiXgbClassifier.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2MultiXgbClassifier.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2NedSNCosmo.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2NedSNCosmo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2NedTap.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2NedTap.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2Observability.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2Observability.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PhaseLimit.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PhaseLimit.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PolynomialFit.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PolynomialFit.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2PropagateStockInfo.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2PropagateStockInfo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RiseDeclineStat.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RiseDeclineStat.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunParsnip.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunParsnip.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunPossis.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunPossis.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunSncosmo.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunSncosmo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunSnoopy.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunSnoopy.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2RunTDE.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2RunTDE.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2TNSEval.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2TNSEval.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/T2XgbClassifier.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/T2XgbClassifier.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t2/xgb_trees.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t2/xgb_trees.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/AbsScoreCalculator.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/AbsScoreCalculator.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/AstroColibriClient.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/AstroColibriClient.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/AstroColibriPublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/AstroColibriPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ChannelSummaryPublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ChannelSummaryPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/CostCounter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/CostCounter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/DCachePublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/DCachePublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ElasticcClassPublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ElasticcClassPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ElasticcTomClient.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ElasticcTomClient.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/HealpixCorrPlotter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/HealpixCorrPlotter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/HealpixTokenGenerator.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/HealpixTokenGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/PlotLightcurveSample.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/PlotLightcurveSample.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/PlotTransientLightcurves.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/PlotTransientLightcurves.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from astropy.cosmology import FlatLambdaCDM
 from astropy.io import fits
 from astropy.table import Table
 from astropy.time import Time
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.colors import Normalize
 from matplotlib.ticker import MultipleLocator
-from slack import WebClient  # type: ignore
+from slack_sdk.web import WebClient
 from ztfquery.utils.stamps import get_ps_stamp  # type: ignore
 
 from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 from ampel.abstract.AbsTabulatedT2Unit import AbsTabulatedT2Unit
 from ampel.content.DataPoint import DataPoint
 from ampel.secret.NamedSecret import NamedSecret
 from ampel.struct.T3Store import T3Store
@@ -523,15 +523,15 @@
 
         # Post to slack
         if self.slack_channel is not None and self.slack_token is not None:
             buffer.seek(0)
             with (
                 open(self.pdf_path, "rb") if self.pdf_path else nullcontext(buffer)  # type: ignore[attr-defined]
             ) as file:
-                self.webclient.files_upload(
+                self.webclient.files_upload_v2(
                     file=file,
                     filename=self.pdf_path or "candidates.pdf",
                     channels=self.slack_channel,
                     #                thread_ts=self.ts,
                 )
 
         return None
```

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RandomMapGenerator.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RandomMapGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RapidBase.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RapidBase.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RapidLco.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RapidLco.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/RapidSedm.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/RapidSedm.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ScoreSingleObject.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ScoreSingleObject.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/ScoreTNSObjects.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/ScoreTNSObjects.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/SlackSummaryPublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/SlackSummaryPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/SubmitTNS.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/SubmitTNS.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TNSMirrorUpdater.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TNSMirrorUpdater.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TransientInfoPrinter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TransientInfoPrinter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TransientTablePublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TransientTablePublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/TransientViewDumper.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/TransientViewDumper.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/VOEventPublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/VOEventPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSClient.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSClient.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSMirrorDB.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSMirrorDB.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/TNSName.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/TNSName.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/t3/tns/tns_ampel_util.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/t3/tns/tns_ampel_util.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_config.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_slackpublisher.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_slackpublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/test/test_t2brightsnprob.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/test/test_t2brightsnprob.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/AmpelHealpix.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/AmpelHealpix.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/automation/get_kn.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/automation/get_kn.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/automation/jobfileCaller.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/automation/jobfileCaller.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/automation/jobfileWriter.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/automation/jobfileWriter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/flatten.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/flatten.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/ampel/contrib/hu/util/ned.py` & `ampel_hu_astro-0.8.4a3/ampel/contrib/hu/util/ned.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/alias.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/alias.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/channel/HU_STELLAR_OUTBURST.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/channel/HU_STELLAR_OUTBURST.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/ChannelSummary.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/ChannelSummary.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/RapidReact.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/StellarPost.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-name: RapidReact
+name: PostOutburst
 tier: 3
 active: true
 template: ztf_periodic_summary
-schedule: every(10).minutes
+schedule: every(60).minutes
 channel:
   any_of:
-    - HU_RAPID_INFANT
+    - HU_STELLAR_OUTBURST
 load:
   - TRANSIENT
   - DATAPOINT
   - T2RECORD
 complement:
   - unit: ZTFCutoutImages
     config:
       eligible: last
   - unit: TNSNames
     config:
       include_report: true
 
-filter: 
-  t2: 
-    unit: T2InfantCatalogEval
-    match: 
-      action: true 
 run:
   - unit: PlotTransientLightcurves
     config:
-      pdf_path: candidates.pdf
-      save_png: true
+      pdf_path: null
+      image_cache_dir: null
+      save_png: false
       include_cutouts: true
-      slack_channel: "#ztf_auto"
+      slack_channel: "#ztf_rapid"
       slack_token:
         label: "slack/ztf_ia/jno"              
       tabulator:
       - unit: ZTFT2Tabulator
   - unit: SkyPortalPublisher
     config:
       groups:
-      - AmpelInfant
+      - AmpelStars
       filters:
-      - AMPEL.HU_RAPID_INFANT
+      - AMPEL.HU_STELLAR_OUTBURST
+      cutouts: null
       token:
         label: fritz/jvs/ampelbot
       base_url: 'https://fritz.science'
-  - unit: SubmitTNS
-    config:
-      tns_submit: true
-      tns_key:
-        label: tns/api/tokendict
```

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/process/StellarPost.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/process/RapidReact.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,53 @@
-name: PostOutburst
+name: RapidReact
 tier: 3
 active: true
 template: ztf_periodic_summary
-schedule: every(60).minutes
+schedule: every(10).minutes
 channel:
   any_of:
-    - HU_STELLAR_OUTBURST
+    - HU_RAPID_INFANT
 load:
   - TRANSIENT
   - DATAPOINT
   - T2RECORD
 complement:
   - unit: ZTFCutoutImages
     config:
       eligible: last
   - unit: TNSNames
     config:
       include_report: true
 
+filter: 
+  t2: 
+    unit: T2InfantCatalogEval
+    match: 
+      action: true 
 run:
   - unit: PlotTransientLightcurves
     config:
       pdf_path: null
-      save_png: true
+      save_png: false
+      image_cache_dir: null
       include_cutouts: true
-      slack_channel: "#ztf_rapid"
+      slack_channel: "#ztf_auto"
       slack_token:
         label: "slack/ztf_ia/jno"              
       tabulator:
       - unit: ZTFT2Tabulator
   - unit: SkyPortalPublisher
     config:
       groups:
-      - AmpelStars
+      - AmpelInfant
       filters:
-      - AMPEL.HU_STELLAR_OUTBURST
+      - AMPEL.HU_RAPID_INFANT
+      cutouts: null
       token:
         label: fritz/jvs/ampelbot
       base_url: 'https://fritz.science'
+  - unit: SubmitTNS
+    config:
+      tns_submit: true
+      tns_key:
+        label: tns/api/tokendict
```

### Comparing `ampel_hu_astro-0.8.4a2/conf/ampel-hu-astro/unit.yml` & `ampel_hu_astro-0.8.4a3/conf/ampel-hu-astro/unit.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a2/pyproject.toml` & `ampel_hu_astro-0.8.4a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-hu-astro"
-version = "0.8.4a2"
+version = "0.8.4a3"
 license = "BSD-3-Clause"
 readme = "README.md"
 description = "Astronomy units for the Ampel system from HU-Berlin"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-HU-astro"
 authors = [
     "Valery Brinnel",
```

### Comparing `ampel_hu_astro-0.8.4a2/PKG-INFO` & `ampel_hu_astro-0.8.4a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampel-hu-astro
-Version: 0.8.4a2
+Version: 0.8.4a3
 Summary: Astronomy units for the Ampel system from HU-Berlin
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

