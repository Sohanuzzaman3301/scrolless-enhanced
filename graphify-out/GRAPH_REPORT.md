# Graph Report - .  (2026-08-01)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 731 nodes · 1189 edges · 57 communities (41 shown, 16 thin omitted)
- Extraction: 93% EXTRACTED · 7% INFERRED · 0% AMBIGUOUS · INFERRED: 87 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `d775736b`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- HomeContent
- ScrollessBlockAccessibilityService
- AutoResizingText
- SessionSegment
- UserSettingsStore
- UserSettingsDao
- BlockableApp
- UserSettingsStoreImpl
- rememberHapticHelper
- SessionSegmentDao
- TimerOverlayManager
- ProgressCard
- HomeViewModel
- TimeProvider
- IntervalTimerState
- TodayBlockingControls
- DebugLogTree
- combine
- BlockOption
- SessionTrackerTest
- BlockingResult
- ScrollessAppState.kt
- AccessibilitySuccessContent
- BlockingManager
- DayLimitBlockHandlerTest
- BlockingManagerImpl
- BlockAllBlockHandlerTest
- NoBlockHandlerTest
- ReviewUtils.kt
- BlockOptionHandler
- DayLimitBlockHandler
- NoBlockHandler
- LocalDateTimeTypeConverters
- LocalDateTypeConverters
- AccessibilitySettingsExt.kt
- gradlew
- requestAppReview
- BaseTest
- BaseTest

## God Nodes (most connected - your core abstractions)
1. `ScrollessBlockAccessibilityService` - 40 edges
2. `UserSettingsDao` - 40 edges
3. `UserSettingsStore` - 40 edges
4. `UserSettingsStoreImpl` - 38 edges
5. `TimerOverlayManager` - 25 edges
6. `SessionSegment` - 25 edges
7. `HomeViewModel` - 23 edges
8. `BlockableApp` - 20 edges
9. `HomeContent()` - 20 edges
10. `ScrollessTheme()` - 19 edges

## Surprising Connections (you probably didn't know these)
- `ProgressCard()` --calls--> `AutoResizingText()`  [INFERRED]
  feature/home/src/main/java/com/scrolless/app/feature/home/components/ProgressCard.kt → core/designsystem/src/main/java/com/scrolless/app/designsystem/component/AutoResizingText.kt
- `FeatureButton()` --calls--> `AutoResizingText()`  [INFERRED]
  feature/home/src/main/java/com/scrolless/app/feature/home/components/TodayBlockingControls.kt → core/designsystem/src/main/java/com/scrolless/app/designsystem/component/AutoResizingText.kt
- `AccessibilityExplainerContent()` --calls--> `AutoResizingText()`  [INFERRED]
  feature/home/src/main/java/com/scrolless/app/feature/home/dialogs/AccessibilityExplainerDialog.kt → core/designsystem/src/main/java/com/scrolless/app/designsystem/component/AutoResizingText.kt
- `HelpDialogContent()` --calls--> `AutoResizingText()`  [INFERRED]
  feature/home/src/main/java/com/scrolless/app/feature/home/dialogs/HelpDialog.kt → core/designsystem/src/main/java/com/scrolless/app/designsystem/component/AutoResizingText.kt
- `ProgressCardPreview()` --calls--> `ScrollessTheme()`  [INFERRED]
  feature/home/src/main/java/com/scrolless/app/feature/home/components/ProgressCard.kt → core/designsystem/src/main/java/com/scrolless/app/designsystem/theme/Theme.kt

## Import Cycles
- None detected.

## Communities (57 total, 16 thin omitted)

### Community 0 - "HomeContent"
Cohesion: 0.08
Nodes (46): MainActivity, Bundle, ComponentActivity, AnimatedIcon(), Modifier, ScrollessTheme(), AccessibilityExplainerBottomSheet(), AccessibilityExplainerBottomSheetPreview() (+38 more)

### Community 1 - "ScrollessBlockAccessibilityService"
Cohesion: 0.09
Nodes (12): AccessibilityEvent, AccessibilityNodeInfo, BlockedContentSession, DetectedBlockedContent, AccessibilityService, ScrollessBlockAccessibilityService, AnyOf, ContentDescriptionPrefix (+4 more)

### Community 2 - "AutoResizingText"
Cohesion: 0.07
Nodes (40): AutoResizingText(), Color, Modifier, WeekdayUsageAverage, analyticsColor(), analyticsDisplayName(), analyticsForDate(), displayName() (+32 more)

### Community 3 - "SessionSegment"
Cohesion: 0.08
Nodes (24): SessionSegmentEntity, toSessionSegment(), Flow, SessionSegmentStoreImpl, SessionSegment, DailyUsageTotal, calculateDailyTotals(), calculateWeekdayAverages() (+16 more)

### Community 4 - "UserSettingsStore"
Cohesion: 0.08
Nodes (3): Flow, setTimerOverlayPosition(), UserSettingsStore

### Community 5 - "UserSettingsDao"
Cohesion: 0.08
Nodes (3): Flow, UserSettingsDao, UserSettingsEntity

### Community 6 - "BlockableApp"
Cohesion: 0.07
Nodes (12): BlockableAppTypeConverters, SessionState, SessionTrackerImpl, BlockableApp, FACEBOOK, FACEBOOK_LITE, REELS, SHORTS (+4 more)

### Community 8 - "rememberHapticHelper"
Cohesion: 0.11
Nodes (23): hapticClickable(), HapticHelper, Modifier, rememberHapticHelper(), PreviewTimeLimitDialog(), TimeLimitDialog(), ExceptReelsSentByDmItem(), Modifier (+15 more)

### Community 9 - "SessionSegmentDao"
Cohesion: 0.09
Nodes (10): BaseDao, Flow, SessionSegmentDao, migrate(), ScrollessDatabase, DataDiModule, Context, RoomDatabase (+2 more)

### Community 10 - "TimerOverlayManager"
Cohesion: 0.12
Nodes (11): android, DragInterceptFrameLayout, Context, ScreenBounds, TimerOverlayManager, FrameLayout, Job, MotionEvent (+3 more)

### Community 11 - "ProgressCard"
Cohesion: 0.14
Nodes (23): AnimatedSegment, AppUsageLegend(), calculateSegments(), Color, Modifier, LegendEntry(), LegendItem, lerp() (+15 more)

### Community 12 - "HomeViewModel"
Cohesion: 0.09
Nodes (7): HomeViewModel, StateFlow, ViewModel, ReviewPromptResult, Shown, SkippedPermanent, SkippedTemporary

### Community 13 - "TimeProvider"
Cohesion: 0.09
Nodes (6): BaseTest, MutableTimeProvider, SessionSegmentStoreImplTest, SystemTimeProvider, TimeProvider, TestSchedulerTimeProvider

### Community 14 - "IntervalTimerState"
Cohesion: 0.25
Nodes (4): IntervalTimerBlockHandler, IntervalTimerState, IntervalTimerBlockHandlerTest, BaseTest

### Community 15 - "TodayBlockingControls"
Cohesion: 0.24
Nodes (17): BlockingButtonType, BLOCK_ALL, DAILY_LIMIT, INTERVAL, ConfigButton(), FeatureButton(), FeatureButtonsRow(), IntervalTimerPointer() (+9 more)

### Community 16 - "DebugLogTree"
Cohesion: 0.15
Nodes (7): ScrollessApplication, Application, DebugLogTree, Timber, Timber, ReleaseLogTree, StackTraceElement

### Community 17 - "combine"
Cohesion: 0.15
Nodes (12): combine(), Flow, R, T1, T2, T3, T4, T5 (+4 more)

### Community 18 - "BlockOption"
Cohesion: 0.18
Nodes (5): BlockOption, BlockAll, DailyLimit, IntervalTimer, NothingSelected

### Community 20 - "BlockingResult"
Cohesion: 0.27
Nodes (5): BlockAllBlockHandler, BlockingResult, BlockNow, CheckLater, Continue

### Community 21 - "ScrollessAppState.kt"
Cohesion: 0.29
Nodes (7): Home, rememberScrollessAppState(), ScrollessAppState, ScrollessRoute, Settings, NavBackStack, NavKey

### Community 22 - "AccessibilitySuccessContent"
Cohesion: 0.27
Nodes (7): AnimatedButton(), Modifier, PopupCircleIcon(), AccessibilitySuccessBottomSheet(), AccessibilitySuccessBottomSheetPreview(), AccessibilitySuccessContent(), NextStep()

### Community 28 - "ReviewUtils.kt"
Cohesion: 0.47
Nodes (5): getInstallerPackageName(), isActivityActive(), Activity, Context, requestAppReview()

### Community 36 - "gradlew"
Cohesion: 0.83
Nodes (3): gradlew script, die(), warn()

## Knowledge Gaps
- **20 isolated node(s):** `BlockAll`, `DailyLimit`, `IntervalTimer`, `NothingSelected`, `REELS` (+15 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **16 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `BlockOption` connect `BlockOption` to `UserSettingsStore`, `ProgressCard`, `HomeViewModel`, `TodayBlockingControls`, `BlockingManager`, `BlockingManagerImpl`?**
  _High betweenness centrality (0.311) - this node is a cross-community bridge._
- **Why does `ScrollessBlockAccessibilityService` connect `ScrollessBlockAccessibilityService` to `TimerOverlayManager`, `UserSettingsStore`, `BlockableApp`, `BlockingManager`?**
  _High betweenness centrality (0.194) - this node is a cross-community bridge._
- **Why does `ProgressCard()` connect `ProgressCard` to `SessionSegment`, `HomeContent`, `AutoResizingText`, `BlockOption`?**
  _High betweenness centrality (0.174) - this node is a cross-community bridge._
- **What connects `BlockAll`, `DailyLimit`, `IntervalTimer` to the rest of the system?**
  _20 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `HomeContent` be split into smaller, more focused modules?**
  _Cohesion score 0.07946127946127945 - nodes in this community are weakly interconnected._
- **Should `ScrollessBlockAccessibilityService` be split into smaller, more focused modules?**
  _Cohesion score 0.09224489795918367 - nodes in this community are weakly interconnected._
- **Should `AutoResizingText` be split into smaller, more focused modules?**
  _Cohesion score 0.06845513413506013 - nodes in this community are weakly interconnected._