# 验收结果

passed-with-deviations(4)

MIR：clean

全部必需检查已通过，主 body BB 全覆盖。公开报告省略本机命令与日志路径。

```json
{
  "status": "passed-with-deviations(4)",
  "passed": true,
  "clean_pass": false,
  "mir_status": "clean",
  "missing_mir_count": 0,
  "counts": {
    "action_count": 8,
    "bb_covered": 244,
    "bb_total": 244,
    "execution_node_count": 13,
    "goal_count": 4,
    "message_count": 17,
    "phase_count": 3
  },
  "browser_checked": true,
  "checks_not_run": [],
  "checks": {
    "batch": {
      "passed": true
    },
    "batch-reference": {
      "passed": true
    },
    "browser": {
      "passed": true
    },
    "contract": {
      "passed": true
    },
    "duplicates": {
      "passed": true
    },
    "hard-rules": {
      "passed": true
    },
    "independent-source": {
      "passed": true
    },
    "principles": {
      "passed": true
    },
    "regressions": {
      "passed": true
    }
  },
  "source_commit": "c248f6d48b97eb4a2aa56147a0b11b7d763278b9",
  "registered_deviation_count": 4,
  "missing_mir": [
    {
      "callee": "std::option::Option::<tools::parallel::ToolCallTimingGuard>::as_mut",
      "category": "declaration",
      "def_path_hash": "0403f53630f0138e2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:157"
    },
    {
      "callee": "<tracing::Level as std::cmp::PartialOrd<tracing::level_filters::LevelFilter>>::le",
      "category": "declaration",
      "def_path_hash": "05ddace4dddbaf572bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2807 (macro)"
    },
    {
      "callee": "<tracing::Level as std::cmp::PartialOrd<tracing::level_filters::LevelFilter>>::le",
      "category": "declaration",
      "def_path_hash": "05ddace4dddbaf572bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2808 (macro)"
    },
    {
      "callee": "<tracing::log::Level as std::cmp::PartialOrd<tracing::log::LevelFilter>>::le",
      "category": "declaration",
      "def_path_hash": "05ddace4dddbaf572bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:3312 (macro)"
    },
    {
      "callee": "tracing::Metadata::<'_>::fields",
      "category": "declaration",
      "def_path_hash": "0a622101c76a53bb5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:74 (macro)"
    },
    {
      "callee": "tracing::Metadata::<'_>::fields",
      "category": "declaration",
      "def_path_hash": "0a622101c76a53bb5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:79 (macro)"
    },
    {
      "callee": "tokio::spawn::<tracing::instrument::Instrumented<{async block@core/src/tools/parallel.rs:197:13: 197:23}>>",
      "category": "declaration",
      "def_path_hash": "12f2d7411dfb7448714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:196"
    },
    {
      "callee": "tracing::__macro_support::__is_enabled",
      "category": "declaration",
      "def_path_hash": "181afd5c325c6bab417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:68 (macro)"
    },
    {
      "callee": "tracing::subscriber::Interest::is_never",
      "category": "declaration",
      "def_path_hash": "266ce036cd642c235f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:67 (macro)"
    },
    {
      "callee": "tracing::level_filters::LevelFilter::current",
      "category": "declaration",
      "def_path_hash": "2cc74db53adc0c125f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2808 (macro)"
    },
    {
      "callee": "tracing::Span::record_all",
      "category": "declaration",
      "def_path_hash": "31ec783950a0ccf7417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:79 (macro)"
    },
    {
      "callee": "tracing::field::FieldSet::value_set_all",
      "category": "declaration",
      "def_path_hash": "476751eea3ab43355f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2977 (macro)"
    },
    {
      "callee": "tracing::field::FieldSet::value_set_all",
      "category": "declaration",
      "def_path_hash": "476751eea3ab43355f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2985 (macro)"
    },
    {
      "callee": "tracing::__macro_support::__disabled_span",
      "category": "declaration",
      "def_path_hash": "5c4a64e746f109da417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:77 (macro)"
    },
    {
      "callee": "tracing::callsite::DefaultCallsite::interest",
      "category": "declaration",
      "def_path_hash": "6141864431f3336c5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:67 (macro)"
    },
    {
      "callee": "tracing::subscriber::Interest::never",
      "category": "declaration",
      "def_path_hash": "669516cd6ffc04035f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:65 (macro)"
    },
    {
      "callee": "<&[std::sync::Arc<dyn codex_extension_api::ToolLifecycleContributor>] as std::iter::IntoIterator>::into_iter",
      "category": "declaration",
      "def_path_hash": "6b7aff59471188cd2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:158 (macro)"
    },
    {
      "callee": "tracing::Span::enter",
      "category": "declaration",
      "def_path_hash": "7a59bdc746a259cf417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:124 (macro)"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:68 (macro)"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:70 (macro)"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:77 (macro)"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:79 (macro)"
    },
    {
      "callee": "<std::slice::Iter<'_, std::sync::Arc<dyn codex_extension_api::ToolLifecycleContributor>> as std::iter::Iterator>::next",
      "category": "declaration",
      "def_path_hash": "8bad2e8350701bdb2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:158 (macro)"
    },
    {
      "callee": "std::option::Option::<tools::parallel::ToolCallTimingGuard>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:167"
    },
    {
      "callee": "<{async block@core/src/tools/parallel.rs:197:13: 197:23} as tracing::Instrument>::in_current_span",
      "category": "declaration",
      "def_path_hash": "a7e1c8b9a4c93bfd417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:197"
    },
    {
      "callee": "<{async block@core/src/tools/parallel.rs:247:9: 247:19} as tracing::Instrument>::in_current_span",
      "category": "declaration",
      "def_path_hash": "a7e1c8b9a4c93bfd417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:247"
    },
    {
      "callee": "tracing::field::display::<&codex_protocol::ThreadId>",
      "category": "declaration",
      "def_path_hash": "b9118929da094bd45f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2836 (macro)"
    },
    {
      "callee": "tracing::field::display::<&codex_protocol::ToolName>",
      "category": "declaration",
      "def_path_hash": "b9118929da094bd45f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2836 (macro)"
    },
    {
      "callee": "std::string::String::as_str",
      "category": "declaration",
      "def_path_hash": "c5047a448ff30a9f0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:191"
    },
    {
      "callee": "std::time::Instant::now",
      "category": "declaration",
      "def_path_hash": "c9a699096f0df9507e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:148"
    },
    {
      "callee": "tracing::dispatcher::has_been_set",
      "category": "declaration",
      "def_path_hash": "d047c8506ef585a05f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:3313 (macro)"
    },
    {
      "callee": "tracing::Span::new",
      "category": "declaration",
      "def_path_hash": "d0f4f0d917049564417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:72 (macro)"
    },
    {
      "callee": "<codex_protocol::ToolName as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:493"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:183"
    },
    {
      "callee": "<std::sync::Arc<codex_extension_api::ExtensionRegistry<config::Config>> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:155"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:143"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:170"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:144"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:172"
    },
    {
      "callee": "<std::sync::Arc<tokio::sync::Mutex<turn_diff_tracker::TurnDiffTracker>> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:145"
    },
    {
      "callee": "<std::sync::Arc<tokio::sync::RwLock<()>> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:146"
    },
    {
      "callee": "<std::sync::Arc<tools::context::ToolCallState> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:173"
    },
    {
      "callee": "<std::sync::Arc<tools::router::ToolRouter> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:142"
    },
    {
      "callee": "<tokio_util::sync::CancellationToken as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:147"
    },
    {
      "callee": "<tools::context::ToolCallSource as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:171"
    },
    {
      "callee": "<tools::router::ToolCall as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:174"
    },
    {
      "callee": "<tracing::Span as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:194"
    },
    {
      "callee": "tokio_util::task::AbortOnDropHandle::<std::result::Result<tools::registry::AnyToolResult, codex_tools::FunctionCallError>>::new",
      "category": "declaration",
      "def_path_hash": "e6f9c4b3b67073ab38787ccc291f4d48",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:196"
    },
    {
      "callee": "<dyn codex_extension_api::ToolLifecycleContributor as codex_extension_api::ToolLifecycleContributor>::on_tool_dispatch",
      "category": "declaration",
      "def_path_hash": "e80cdd8092b4cacff696af05e8b8761e",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/parallel.rs:159"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:152"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:160"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:161"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:162"
    },
    {
      "callee": "<std::sync::Arc<codex_extension_api::ExtensionRegistry<config::Config>> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:158"
    },
    {
      "callee": "<std::sync::Arc<dyn codex_extension_api::ToolLifecycleContributor> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:159"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:134"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:135"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:151"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:155"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:158"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:175"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:190"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:138"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:139"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:144"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:152"
    },
    {
      "callee": "<std::sync::Arc<tools::router::ToolRouter> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/executed_tool_calls.rs:351"
    },
    {
      "callee": "<std::sync::Arc<tools::router::ToolRouter> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:140"
    },
    {
      "callee": "<std::sync::Arc<tools::router::ToolRouter> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:141"
    },
    {
      "callee": "std::option::Option::<&tools::parallel::ToolCallTimingGuard>::map::<std::sync::Arc<std::sync::OnceLock<std::time::Instant>>, {closure@core/src/tools/parallel.rs:169:18: 169:26}>",
      "category": "declaration",
      "def_path_hash": "efc1704abda0d2442bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/parallel.rs:167"
    }
  ]
}
```
