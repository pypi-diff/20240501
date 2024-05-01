# Comparing `tmp/aliceio-0.0.2.tar.gz` & `tmp/aliceio-0.0.3.tar.gz`

## Comparing `aliceio-0.0.2.tar` & `aliceio-0.0.3.tar`

### file list

```diff
@@ -1,418 +1,423 @@
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 aliceio-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 aliceio-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0    11590 2020-02-02 00:00:00.000000 aliceio-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 aliceio-0.0.2/.github/pull_request_template.md
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 aliceio-0.0.2/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aliceio-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aliceio-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aliceio-0.0.2/.github/workflows/pypi-release.yml
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 aliceio-0.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/__meta__.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/exceptions.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/loggers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/__init__.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/alice.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/context_controller.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/skill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/__init__.py
--rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/aiohttp.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/middlewares/__init__.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/middlewares/base.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/middlewares/manager.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/client/session/middlewares/request_logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/__init__.py
--rw-r--r--   0        0        0    13807 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/dispatcher.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/flags.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/event/__init__.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/event/alice.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/event/bases.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/event/event.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/event/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/middlewares/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/middlewares/base.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/middlewares/error.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/middlewares/manager.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/middlewares/response_convert.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/dispatcher/middlewares/user_context.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/audio_error.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/base.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/card.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/entity.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/file_type.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/http_method.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/enums/update.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/filters/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/filters/base.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/filters/exception.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/filters/logic.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/filters/magic_data.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/filters/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/__init__.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/context.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/state.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/strategy.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/middlewares/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/middlewares/api_storage.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/middlewares/fsm_context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/storage/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/storage/api.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/storage/base.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/storage/memory.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/fsm/storage/redis.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/audio_player.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/base.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/button_pressed.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/error.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/message.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/purchase.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/show_pull.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/handlers/timeout.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/base.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/status.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/images/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/images/delete_image.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/images/get_images.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/images/upload_image.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/sounds/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/sounds/delete_sound.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/sounds/get_sounds.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/methods/sounds/upload_sound.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/alice_event.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/alice_request.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/alice_response.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/analytic_event.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/analytics.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/api_state.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/application.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/audio_player.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/audio_player_directive.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/audio_player_error.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/audio_player_item.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/base.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/big_image.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/button_pressed.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/card.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/card_footer.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/card_header.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/datetime.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/directives.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/entity.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/error_event.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/error_result.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/fio_entity.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/geo_entity.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/image_gallery.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/image_gallery_item.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/input_file.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/interfaces.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/item_image.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/items_list.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/markup.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/media_button.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/message.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/meta.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/metadata.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/nlu.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/nlu_entity.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/number_entity.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/payload.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/purchase.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/quota.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/response.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/result.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/session.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/show_item_meta.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/show_pull.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/space_status.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/stream.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/text_button.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/timeout_event.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/tokens_entity.py
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/update.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/uploaded_image.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/uploaded_sound.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/url.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/types/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/utils/__init__.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/utils/builders.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/utils/funcs.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/utils/magic_filter.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/utils/mixins.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/utils/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/webhook/__init__.py
--rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/webhook/aiohttp_server.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 aliceio-0.0.2/aliceio/webhook/security.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_config.yml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/index.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/install.md
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_css/style.css
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/alice-skill.png
--rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/create-dialog.png
--rw-r--r--   0        0        0   192775 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/logo-aliceio-black-text.png
--rw-r--r--   0        0        0   171494 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/logo-aliceio-black.png
--rw-r--r--   0        0        0   295360 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/logo-aliceio-trans-text.png
--rw-r--r--   0        0        0   239699 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/logo-aliceio-trans.png
--rw-r--r--   0        0        0   181025 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/logo-aliceio-white-text.png
--rw-r--r--   0        0        0   163665 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/logo-aliceio-white.png
--rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/middleware-dark.png
--rw-r--r--   0        0        0    52245 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/middleware-light.png
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/ngrok.png
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/save-settings.png
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/skill-id-url.png
--rw-r--r--   0        0        0    18794 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/skill-id.png
--rw-r--r--   0        0        0    28437 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/skill-settings.png
--rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/_static/testing.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/alice.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/context-controller.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/skill.md
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/session/aiohttp.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/session/base.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/session/middlewares/base.md
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/session/middlewares/manager.md
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/client/session/middlewares/request-logging.md
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/dispatcher.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/flags.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/router.md
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/event/alice.md
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/event/bases.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/event/event.md
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/event/handler.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/middlewares/base.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/middlewares/error.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/middlewares/manager.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/middlewares/response-convert.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/dispatcher/middlewares/user-context.md
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/enums/all-enums.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/filters/base.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/filters/exception.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/filters/logic.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/filters/magic-data.md
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/filters/magic-filter.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/filters/state.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/context.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/state.md
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/strategy.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/middlewares/api-storage.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/middlewares/fsm-context.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/storage/api.md
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/storage/base.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/storage/memory.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/storage/redis/default-key-builder.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/storage/redis/key-builder.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/fsm/storage/redis/redis.md
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/audio-player.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/base.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/button-pressed.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/error.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/message.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/purchase.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/show-pull.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/handlers/timeout.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/base.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/status.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/images/delete-image.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/images/get-images.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/images/upload-image.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/sounds/delete-sound.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/sounds/get-sounds.md
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/methods/sounds/upload-sound.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/alice-event.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/alice-request.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/alice-response.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/analytic-event.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/analytics.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/api-state.md
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/application.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/audio-player-directive.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/audio-player-error.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/audio-player-item.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/audio-player.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/base.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/big-image.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/button-pressed.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/card-footer.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/card-header.md
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/card.md
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/datetime.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/directives.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/entity.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/error-event.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/error-result.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/fio-entity.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/geo-entity.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/image-gallery-item.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/image-gallery.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/input-file.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/interfaces.md
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/item-image.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/items-list.md
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/markup.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/media-button.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/message.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/meta.md
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/metadata.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/nlu-entity.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/nlu.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/number-entity.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/payload.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/purchase.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/quota.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/response.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/result.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/session.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/show-item-meta.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/show-pull.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/space-status.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/stream.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/text-button.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/timeout-event.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/tokens-entity.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/update.md
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/uploaded-image.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/uploaded-sound.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/url.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/types/user.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/builders.md
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/funcs.md
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/mixins.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/warnings.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/builders/builder.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/builders/image-gallery-builder.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/builders/items-list-builder.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/utils/builders/text-button-builder.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/webhook/aiohttp-server.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/aliceio/webhook/security.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/templates/python/material/languages/en.html
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/builders.md
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/dependency-injection.md
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/error-handling.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/faq.md
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/filters.md
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/finite-state-machine.md
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/first-skill.md
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/full-skill.md
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/index.md
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/methods.md
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/middlewares.md
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/routers.md
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/special-events.md
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 aliceio-0.0.2/docs/tutorial/start.md
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/builders.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/buy_elephant.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/context_addition.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/echo_skill.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/echo_skill_ssl.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/error_handling.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/fast_start.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/filters.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/fsm_form.py
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/fsm_games.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/methods.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/middlewares.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/special_events.py
--rw-r--r--   0        0        0   345847 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/data/watermelon.png
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/data/watermelon_rip.mp3
--rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/data/watermelon_rip2.mp3
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/multi_file_skill/skill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/multi_file_skill/handlers/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/multi_file_skill/handlers/echo.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/multi_file_skill/handlers/ping.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aliceio-0.0.2/examples/multi_file_skill/handlers/start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/docker-compose.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/mocked/__init__.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/mocked/mocked_skill.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/mocked/mocked_update.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/__init__.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_alice_server.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_context_controller.py
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_skill.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_session/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_session/test_aiohttp_session.py
--rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_session/test_base_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_session/test_middlewares/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_session/test_middlewares/test_manager.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_client/test_session/test_middlewares/test_request_logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_methods/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_alice_event.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_audio_player_directive.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_card.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_entity.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_error_event.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_input_file.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_message.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_quota.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_timeout_event.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_update.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_api/test_types/test_uploaded.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/__init__.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_dispatcher.py
--rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_router.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_timeout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_event/__init__.py
--rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_event/test_alice.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_event/test_event.py
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_event/test_handler.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_event/test_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_middlewares/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_middlewares/test_error.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_middlewares/test_response_converter.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_dispatcher/test_middlewares/test_user_context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_filters/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_filters/test_base.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_filters/test_exception.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_filters/test_logic.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_filters/test_magic_data.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_filters/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_flags/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_flags/test_decorator.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_flags/test_getter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/__init__.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/test_context.py
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/test_state.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/test_strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/middlewares/__init__.py
--rw-r--r--   0        0        0    10124 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/middlewares/test_api_storage.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/middlewares/test_fsm_context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/storage/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/storage/test_redis.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_fsm/storage/test_storages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_audio_player.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_base.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_button_pressed.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_error.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_message.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_purchase.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_show_pull.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_handlers/test_timeout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_methods/__init__.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_methods/test_base.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_methods/test_images.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_methods/test_sounds.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_methods/test_status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_utils/test_builders.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_utils/test_exceptions.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_utils/test_magic_filter.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_utils/test_mixins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_webhook/__init__.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_webhook/test_aiohttp_server.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 aliceio-0.0.2/tests/test_webhook/test_security.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aliceio-0.0.2/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 aliceio-0.0.2/LICENSE
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aliceio-0.0.2/NOTICE
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 aliceio-0.0.2/README.md
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aliceio-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 aliceio-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 aliceio-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 aliceio-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aliceio-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aliceio-0.0.3/codecov.yml
+-rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 aliceio-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 aliceio-0.0.3/.github/pull_request_template.md
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 aliceio-0.0.3/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aliceio-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aliceio-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aliceio-0.0.3/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 aliceio-0.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/__meta__.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/exceptions.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/loggers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/__init__.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/alice.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/context_controller.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/skill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/__init__.py
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/aiohttp.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/middlewares/__init__.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/middlewares/base.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/middlewares/manager.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/client/session/middlewares/request_logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/__init__.py
+-rw-r--r--   0        0        0    14100 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/dispatcher.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/flags.py
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/event/__init__.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/event/alice.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/event/bases.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/event/event.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/event/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/middlewares/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/middlewares/base.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/middlewares/error.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/middlewares/manager.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/middlewares/response_convert.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/dispatcher/middlewares/user_context.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/audio_error.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/base.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/card.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/entity.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/file_type.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/http_method.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/enums/update.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/filters/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/filters/base.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/filters/exception.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/filters/logic.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/filters/magic_data.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/filters/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/__init__.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/context.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/state.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/strategy.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/middlewares/__init__.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/middlewares/api_storage.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/middlewares/fsm_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/storage/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/storage/api.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/storage/base.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/storage/memory.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/fsm/storage/redis.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/audio_player.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/base.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/button_pressed.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/error.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/message.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/purchase.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/show_pull.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/handlers/timeout.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/base.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/status.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/images/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/images/delete_image.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/images/get_images.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/images/upload_image.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/sounds/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/sounds/delete_sound.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/sounds/get_sounds.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/methods/sounds/upload_sound.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/alice_event.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/alice_request.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/alice_response.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/analytic_event.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/analytics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/api_state.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/application.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/audio_player.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/audio_player_directive.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/audio_player_error.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/audio_player_item.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/base.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/big_image.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/button_pressed.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/card.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/card_footer.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/card_header.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/datetime.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/directives.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/entity.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/error_event.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/error_result.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/fio_entity.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/geo_entity.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/image_gallery.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/image_gallery_item.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/input_file.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/interfaces.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/item_image.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/items_list.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/markup.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/media_button.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/message.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/meta.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/metadata.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/nlu.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/nlu_entity.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/number_entity.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/payload.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/purchase.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/quota.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/response.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/result.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/session.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/show_item_meta.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/show_pull.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/space_status.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/stream.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/text_button.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/timeout_event.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/tokens_entity.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/update.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/uploaded_image.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/uploaded_sound.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/url.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/types/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/utils/__init__.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/utils/builders.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/utils/funcs.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/utils/magic_filter.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/utils/mixins.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/utils/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/webhook/__init__.py
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/webhook/aiohttp_server.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 aliceio-0.0.3/aliceio/webhook/security.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_config.yml
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/contributing.md
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/index.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/install.md
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_css/style.css
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/alice-skill.png
+-rw-r--r--   0        0        0    31178 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/alice-storage.png
+-rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/create-dialog.png
+-rw-r--r--   0        0        0   192775 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/logo-aliceio-black-text.png
+-rw-r--r--   0        0        0   171494 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/logo-aliceio-black.png
+-rw-r--r--   0        0        0   295360 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/logo-aliceio-trans-text.png
+-rw-r--r--   0        0        0   239699 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/logo-aliceio-trans.png
+-rw-r--r--   0        0        0   181025 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/logo-aliceio-white-text.png
+-rw-r--r--   0        0        0   163665 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/logo-aliceio-white.png
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/middleware-dark.png
+-rw-r--r--   0        0        0    52245 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/middleware-light.png
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/ngrok.png
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/save-settings.png
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/skill-id-url.png
+-rw-r--r--   0        0        0    18794 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/skill-id.png
+-rw-r--r--   0        0        0    28437 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/skill-settings.png
+-rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/_static/testing.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/alice.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/context-controller.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/skill.md
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/session/aiohttp.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/session/base.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/session/middlewares/base.md
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/session/middlewares/manager.md
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/client/session/middlewares/request-logging.md
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/dispatcher.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/flags.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/router.md
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/event/alice.md
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/event/bases.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/event/event.md
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/event/handler.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/middlewares/base.md
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/middlewares/error.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/middlewares/manager.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/middlewares/response-convert.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/dispatcher/middlewares/user-context.md
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/enums/all-enums.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/filters/base.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/filters/exception.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/filters/logic.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/filters/magic-data.md
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/filters/magic-filter.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/filters/state.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/context.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/state.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/strategy.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/middlewares/api-storage.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/middlewares/fsm-context.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/storage/api.md
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/storage/base.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/storage/memory.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/storage/redis/default-key-builder.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/storage/redis/key-builder.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/fsm/storage/redis/redis.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/audio-player.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/base.md
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/button-pressed.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/error.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/message.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/purchase.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/show-pull.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/handlers/timeout.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/base.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/status.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/images/delete-image.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/images/get-images.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/images/upload-image.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/sounds/delete-sound.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/sounds/get-sounds.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/methods/sounds/upload-sound.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/alice-event.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/alice-request.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/alice-response.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/analytic-event.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/analytics.md
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/api-state.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/application.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/audio-player-directive.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/audio-player-error.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/audio-player-item.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/audio-player.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/base.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/big-image.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/button-pressed.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/card-footer.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/card-header.md
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/card.md
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/datetime.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/directives.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/entity.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/error-event.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/error-result.md
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/fio-entity.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/geo-entity.md
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/image-gallery-item.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/image-gallery.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/input-file.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/interfaces.md
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/item-image.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/items-list.md
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/markup.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/media-button.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/message.md
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/meta.md
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/metadata.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/nlu-entity.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/nlu.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/number-entity.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/payload.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/purchase.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/quota.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/response.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/result.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/session.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/show-item-meta.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/show-pull.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/space-status.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/stream.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/text-button.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/timeout-event.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/tokens-entity.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/update.md
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/uploaded-image.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/uploaded-sound.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/url.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/types/user.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/builders.md
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/funcs.md
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/mixins.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/warnings.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/builders/builder.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/builders/image-gallery-builder.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/builders/items-list-builder.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/utils/builders/text-button-builder.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/webhook/aiohttp-server.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/aliceio/webhook/security.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/templates/python/material/languages/en.html
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/builders.md
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/dependency-injection.md
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/error-handling.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/faq.md
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/filters.md
+-rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/finite-state-machine.md
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/first-skill.md
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/full-skill.md
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/index.md
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/methods.md
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/middlewares.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/routers.md
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/special-events.md
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 aliceio-0.0.3/docs/tutorial/start.md
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/builders.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/buy_elephant.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/context_addition.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/echo_skill.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/echo_skill_ssl.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/error_handling.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/fast_start.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/filters.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/fsm_form.py
+-rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/fsm_games.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/methods.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/middlewares.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/special_events.py
+-rw-r--r--   0        0        0   345847 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/data/watermelon.png
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/data/watermelon_rip.mp3
+-rw-r--r--   0        0        0    11701 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/data/watermelon_rip2.mp3
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/multi_file_skill/skill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/multi_file_skill/handlers/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/multi_file_skill/handlers/echo.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/multi_file_skill/handlers/ping.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aliceio-0.0.3/examples/multi_file_skill/handlers/start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/docker-compose.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/mocked/__init__.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/mocked/mocked_skill.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/mocked/mocked_update.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/__init__.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_alice_server.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_context_controller.py
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_skill.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_session/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_session/test_aiohttp_session.py
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_session/test_base_session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_session/test_middlewares/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_session/test_middlewares/test_manager.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_client/test_session/test_middlewares/test_request_logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_methods/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_alice_event.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_audio_player_directive.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_card.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_entity.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_error_event.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_input_file.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_message.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_quota.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_session.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_timeout_event.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_update.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_api/test_types/test_uploaded.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/__init__.py
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_dispatcher.py
+-rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_router.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_timeout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_event/__init__.py
+-rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_event/test_alice.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_event/test_event.py
+-rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_event/test_handler.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_event/test_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_middlewares/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_middlewares/test_error.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_middlewares/test_response_converter.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_dispatcher/test_middlewares/test_user_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_filters/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_filters/test_base.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_filters/test_exception.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_filters/test_logic.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_filters/test_magic_data.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_filters/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_flags/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_flags/test_decorator.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_flags/test_getter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/__init__.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/test_context.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/test_state.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/test_strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/middlewares/__init__.py
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/middlewares/test_api_storage.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/middlewares/test_fsm_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/storage/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/storage/test_redis.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_fsm/storage/test_storages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_audio_player.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_base.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_button_pressed.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_error.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_message.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_purchase.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_show_pull.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_handlers/test_timeout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_methods/__init__.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_methods/test_base.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_methods/test_images.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_methods/test_sounds.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_methods/test_status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_utils/test_builders.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_utils/test_exceptions.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_utils/test_magic_filter.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_utils/test_mixins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_webhook/__init__.py
+-rw-r--r--   0        0        0    17089 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_webhook/test_aiohttp_server.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 aliceio-0.0.3/tests/test_webhook/test_security.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aliceio-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 aliceio-0.0.3/LICENSE
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aliceio-0.0.3/NOTICE
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 aliceio-0.0.3/README.md
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aliceio-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 aliceio-0.0.3/PKG-INFO
```

### Comparing `aliceio-0.0.2/.pre-commit-config.yaml` & `aliceio-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/mkdocs.yml` & `aliceio-0.0.3/mkdocs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 copyright: <a href="https://github.com/K1rL3s/aliceio/tree/master/LICENSE" target="_blank" rel="noopener">Лицензия</a>
 
 extra:
   generator: false
   disqus: ""
   social:
     - icon: fontawesome/brands/telegram
-      link: https://t.me/aliceio_ru
+      link: https://t.me/aliceio_chat
       name: Наш ТГ чат
 
 nav:
   - Документация:
       - index.md
       - Установка: install.md
       - API Алисы:
@@ -160,14 +160,15 @@
               - ResponseConvert: aliceio/dispatcher/middlewares/response-convert.md
               - FSMContextMiddleware: aliceio/fsm/middlewares/fsm-context.md
               - FSMApiStorageMiddleware: aliceio/fsm/middlewares/api-storage.md
           - Утилсы:
               - Funcs: aliceio/utils/funcs.md
               - Mixins: aliceio/utils/mixins.md
               - Warnings: aliceio/utils/warnings.md
+      - Контрибьютинг: contributing.md
 
   - Туториал:
       - tutorial/index.md
       - Начало: tutorial/start.md
       - Первый навык: tutorial/first-skill.md
       - Методы API: tutorial/methods.md
       - Роутеры: tutorial/routers.md
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 site_name: AliceIO Docs site_author: AliceIO site_description: Awesome Alice
 framework site_url: https://aliceio.rtfd.io/ru/latest/ repo_name: aliceio
 repo_url: https://github.com/K1rL3s/aliceio edit_uri: edit/master/docs/
 copyright: _Ð__Ð_¸_Ñ__Ð_µ_Ð_½_Ð_·_Ð_¸_Ñ_ extra: generator: false disqus: "" social: - icon:
-fontawesome/brands/telegram link: https://t.me/aliceio_ru name: ÐÐ°Ñ Ð¢Ð
+fontawesome/brands/telegram link: https://t.me/aliceio_chat name: ÐÐ°Ñ Ð¢Ð
 ÑÐ°Ñ nav: - ÐÐ¾ÐºÑÐ¼ÐµÐ½ÑÐ°ÑÐ¸Ñ: - index.md - Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ°:
 install.md - API ÐÐ»Ð¸ÑÑ: - ÐÐ°Ð²ÑÐº: aliceio/client/skill.md - Enums:
 aliceio/enums/all-enums.md - ÐÐµÑÐ¾Ð´Ñ: - Base: aliceio/methods/base.md -
 Ð¡ÑÐ°ÑÑÑ: aliceio/methods/status.md - ÐÐ·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ: -
 ÐÐ°Ð³ÑÑÐ·Ð¸ÑÑ: aliceio/methods/images/upload-image.md - ÐÐ¾Ð»ÑÑÐ¸ÑÑ:
 aliceio/methods/images/get-images.md - Ð£Ð´Ð°Ð»Ð¸ÑÑ: aliceio/methods/images/
 delete-image.md - ÐÐ²ÑÐºÐ¸: - ÐÐ°Ð³ÑÑÐ·Ð¸ÑÑ: aliceio/methods/sounds/
@@ -79,39 +79,39 @@
 aliceio/dispatcher/event/handler.md - ÐÐ¸Ð´Ð»Ð²Ð°ÑÐ¸: - Manager: aliceio/
 dispatcher/middlewares/manager.md - UserContext: aliceio/dispatcher/
 middlewares/user-context.md - Error: aliceio/dispatcher/middlewares/error.md -
 ResponseConvert: aliceio/dispatcher/middlewares/response-convert.md -
 FSMContextMiddleware: aliceio/fsm/middlewares/fsm-context.md -
 FSMApiStorageMiddleware: aliceio/fsm/middlewares/api-storage.md - Ð£ÑÐ¸Ð»ÑÑ:
 - Funcs: aliceio/utils/funcs.md - Mixins: aliceio/utils/mixins.md - Warnings:
-aliceio/utils/warnings.md - Ð¢ÑÑÐ¾ÑÐ¸Ð°Ð»: - tutorial/index.md -
-ÐÐ°ÑÐ°Ð»Ð¾: tutorial/start.md - ÐÐµÑÐ²ÑÐ¹ Ð½Ð°Ð²ÑÐº: tutorial/first-
-skill.md - ÐÐµÑÐ¾Ð´Ñ API: tutorial/methods.md - Ð Ð¾ÑÑÐµÑÑ: tutorial/
-routers.md - Ð¤Ð¸Ð»ÑÑÑÑ: tutorial/filters.md - ÐÐ¸Ð´Ð»Ð²Ð°ÑÐ¸: tutorial/
-middlewares.md - ÐÐ°ÑÐ¸Ð½Ð° ÑÐ¾ÑÑÐ¾ÑÐ½Ð¸Ð¹: tutorial/finite-state-
-machine.md - ÐÐ½Ð¾Ð¿ÐºÐ¸ Ð¸ Ð°Ð»ÑÐ±Ð¾Ð¼Ñ: tutorial/builders.md -
-ÐÐ±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð¾ÑÐ¸Ð±Ð¾Ðº: tutorial/error-handling.md - ÐÑÐ¾Ð±ÑÐµ
-ÑÐ¾Ð±ÑÑÐ¸Ñ: tutorial/special-events.md - ÐÐ½ÐµÐ´ÑÐµÐ½Ð¸Ðµ
-Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐµÐ¹: tutorial/dependency-injection.md -
-ÐÐ¾Ð»Ð½Ð¾ÑÐµÐ½Ð½ÑÐ¹ Ð½Ð°Ð²ÑÐº: tutorial/full-skill.md - FAQ: tutorial/
-faq.md theme: name: material language: ru features: - navigation.instant -
-navigation.indexes - navigation.tracking - navigation.tabs - navigation.top -
-search.suggest - content.code.copy palette: - media: "(prefers-color-scheme:
-light)" scheme: default accent: blue toggle: icon: material/toggle-switch name:
-Switch to dark mode - media: "(prefers-color-scheme: dark)" scheme: slate
-accent: blue toggle: icon: material/toggle-switch-off-outline name: Switch to
-light mode font: text: Roboto Mono code: Monaco logo: _static/logo-aliceio-
-trans.png favicon: _static/logo-aliceio-trans.png markdown_extensions: -
-attr_list: - admonition: - md_in_html: - pymdownx.magiclink:
-repo_url_shortener: true repo_url_shorthand: true normalize_issue_symbols: true
-user: K1rL3s repo: aliceio - pymdownx.highlight: anchor_linenums: true
-line_spans: __span pygments_lang_class: true linenums: true guess_lang: true -
-pymdownx.inlinehilite: - pymdownx.superfences: - pymdownx.tabbed:
-alternate_style: true - pymdownx.escapeall: hardbreak: True nbsp: True -
-pymdownx.details: - pymdownx.tabbed: - pymdownx.saneheaders: plugins: - search:
-- mkdocstrings: custom_templates: docs/templates handlers: python: options:
-docstring_options: ignore_init_summary: false trim_doctest_flags: true
-docstring_section_style: list docstring_style: sphinx group_by_category: true
-show_docstring_description: true merge_init_into_class: false
-show_root_heading: true show_signature: true show_signature_annotations: true
-show_source: false show_symbol_type_heading: true show_symbol_type_toc: true
-extra_css: - _css/style.css
+aliceio/utils/warnings.md - ÐÐ¾Ð½ÑÑÐ¸Ð±ÑÑÑÐ¸Ð½Ð³: contributing.md -
+Ð¢ÑÑÐ¾ÑÐ¸Ð°Ð»: - tutorial/index.md - ÐÐ°ÑÐ°Ð»Ð¾: tutorial/start.md -
+ÐÐµÑÐ²ÑÐ¹ Ð½Ð°Ð²ÑÐº: tutorial/first-skill.md - ÐÐµÑÐ¾Ð´Ñ API: tutorial/
+methods.md - Ð Ð¾ÑÑÐµÑÑ: tutorial/routers.md - Ð¤Ð¸Ð»ÑÑÑÑ: tutorial/
+filters.md - ÐÐ¸Ð´Ð»Ð²Ð°ÑÐ¸: tutorial/middlewares.md - ÐÐ°ÑÐ¸Ð½Ð°
+ÑÐ¾ÑÑÐ¾ÑÐ½Ð¸Ð¹: tutorial/finite-state-machine.md - ÐÐ½Ð¾Ð¿ÐºÐ¸ Ð¸
+Ð°Ð»ÑÐ±Ð¾Ð¼Ñ: tutorial/builders.md - ÐÐ±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð¾ÑÐ¸Ð±Ð¾Ðº:
+tutorial/error-handling.md - ÐÑÐ¾Ð±ÑÐµ ÑÐ¾Ð±ÑÑÐ¸Ñ: tutorial/special-
+events.md - ÐÐ½ÐµÐ´ÑÐµÐ½Ð¸Ðµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐµÐ¹: tutorial/dependency-
+injection.md - ÐÐ¾Ð»Ð½Ð¾ÑÐµÐ½Ð½ÑÐ¹ Ð½Ð°Ð²ÑÐº: tutorial/full-skill.md - FAQ:
+tutorial/faq.md theme: name: material language: ru features: -
+navigation.instant - navigation.indexes - navigation.tracking - navigation.tabs
+- navigation.top - search.suggest - content.code.copy palette: - media: "
+(prefers-color-scheme: light)" scheme: default accent: blue toggle: icon:
+material/toggle-switch name: Switch to dark mode - media: "(prefers-color-
+scheme: dark)" scheme: slate accent: blue toggle: icon: material/toggle-switch-
+off-outline name: Switch to light mode font: text: Roboto Mono code: Monaco
+logo: _static/logo-aliceio-trans.png favicon: _static/logo-aliceio-trans.png
+markdown_extensions: - attr_list: - admonition: - md_in_html: -
+pymdownx.magiclink: repo_url_shortener: true repo_url_shorthand: true
+normalize_issue_symbols: true user: K1rL3s repo: aliceio - pymdownx.highlight:
+anchor_linenums: true line_spans: __span pygments_lang_class: true linenums:
+true guess_lang: true - pymdownx.inlinehilite: - pymdownx.superfences: -
+pymdownx.tabbed: alternate_style: true - pymdownx.escapeall: hardbreak: True
+nbsp: True - pymdownx.details: - pymdownx.tabbed: - pymdownx.saneheaders:
+plugins: - search: - mkdocstrings: custom_templates: docs/templates handlers:
+python: options: docstring_options: ignore_init_summary: false
+trim_doctest_flags: true docstring_section_style: list docstring_style: sphinx
+group_by_category: true show_docstring_description: true merge_init_into_class:
+false show_root_heading: true show_signature: true show_signature_annotations:
+true show_source: false show_symbol_type_heading: true show_symbol_type_toc:
+true extra_css: - _css/style.css
```

### Comparing `aliceio-0.0.2/.github/pull_request_template.md` & `aliceio-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/.github/ISSUE_TEMPLATE/bug.yml` & `aliceio-0.0.3/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml` & `aliceio-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/.github/workflows/pypi-release.yml` & `aliceio-0.0.3/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/.github/workflows/tests.yml` & `aliceio-0.0.3/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: pyproject.toml
 
       - name: Install project dependencies
         run: |
-          pip install -e .[dev,test,redis,proxy,i18n,fast]
+          pip install -e .[dev,test,redis,proxy,fast]
 
       - name: Lint code
         run: |
           ruff --output-format=github aliceio examples
           mypy aliceio
           black --check --diff aliceio tests
 
@@ -78,22 +78,22 @@
 
       - name: Run tests
         run: |
           flags="$flags --cov=aliceio --cov-config .coveragerc --cov-report=xml"
           [[ "$IS_WINDOWS" == "false" ]] && flags="$flags --redis redis://localhost:6379/0"
           pytest $flags
 
-  #      - name: Upload coverage data
-  #        uses: codecov/codecov-action@v3
-  #        with:
-  #          token: ${{ secrets.CODECOV_TOKEN }}
-  #          files: coverage.xml
-  #          flags: unittests
-  #          name: py-${{ matrix.python-version }}-${{ matrix.os }}
-  #          fail_ci_if_error: true
+      - name: Upload coverage data
+        uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          files: coverage.xml
+          flags: unittests
+          name: py-${{ matrix.python-version }}-${{ matrix.os }}
+          fail_ci_if_error: true
 
   pypy-tests:
     strategy:
       fail-fast: false
       matrix:
         os:
           - ubuntu-latest
@@ -119,15 +119,15 @@
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: pyproject.toml
 
       - name: Install project dependencies
         run: |
-          pip install -e .[dev,test,redis,proxy,i18n,fast]
+          pip install -e .[dev,test,redis,proxy,fast]
 
       - name: Setup redis
         uses: shogo82148/actions-setup-redis@v1
         with:
           redis-version: 7
 
       - name: Run tests
```

### Comparing `aliceio-0.0.2/aliceio/__init__.py` & `aliceio-0.0.3/aliceio/__init__.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/exceptions.py` & `aliceio-0.0.3/aliceio/exceptions.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/alice.py` & `aliceio-0.0.3/aliceio/client/alice.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/context_controller.py` & `aliceio-0.0.3/aliceio/client/context_controller.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/skill.py` & `aliceio-0.0.3/aliceio/client/skill.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/session/aiohttp.py` & `aliceio-0.0.3/aliceio/client/session/aiohttp.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/session/base.py` & `aliceio-0.0.3/aliceio/client/session/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/session/middlewares/base.py` & `aliceio-0.0.3/aliceio/client/session/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/session/middlewares/manager.py` & `aliceio-0.0.3/aliceio/client/session/middlewares/manager.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/client/session/middlewares/request_logging.py` & `aliceio-0.0.3/aliceio/client/session/middlewares/request_logging.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/dispatcher.py` & `aliceio-0.0.3/aliceio/dispatcher/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.update.outer_middleware(ErrorsMiddleware(self))
 
         # UserContextMiddleware выполняет небольшую оптимизацию
         # для всех других встроенных мидлварей путем кэширования
         # экземпляров пользователя и сессиив контексте событий.
         self.update.outer_middleware(UserContextMiddleware())
 
-        storage = self._init_storage(storage, disable_fsm, use_api_storage)
+        storage = self._create_storage(storage, disable_fsm, use_api_storage)
         # FSMContextMiddleware всегда следует регистрировать после UserContextMiddleware
         # поскольку здесь используется контекст из предыдущего шага.
         self.fsm = FSMContextMiddleware(
             storage=storage,
             strategy=fsm_strategy,
         )
         if not disable_fsm:
@@ -122,16 +122,19 @@
     def parent_router(self, value: Router) -> None:
         """
         Диспетчер является корневым маршрутизатором,
         поэтому ему нельзя настроить родительский роутер.
         """
         raise RuntimeError("Dispatcher can not be attached to another Router.")
 
+    # Правильнее всего будет оставить только одно условие `storage is not None`,
+    # а после возвращать MemoryStorage. Но что-то может произойти с ApiStorage'ом,
+    # поэтому пока так
     @staticmethod
-    def _init_storage(
+    def _create_storage(
         storage: Optional[BaseStorage],
         disable_fsm: bool,
         use_api_storage: bool,
     ) -> BaseStorage:
         if storage is not None:
             return storage
         if disable_fsm:
```

### Comparing `aliceio-0.0.2/aliceio/dispatcher/flags.py` & `aliceio-0.0.3/aliceio/dispatcher/flags.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/router.py` & `aliceio-0.0.3/aliceio/dispatcher/router.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/event/alice.py` & `aliceio-0.0.3/aliceio/dispatcher/event/alice.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/event/bases.py` & `aliceio-0.0.3/aliceio/dispatcher/event/bases.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/event/event.py` & `aliceio-0.0.3/aliceio/dispatcher/event/event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/event/handler.py` & `aliceio-0.0.3/aliceio/dispatcher/event/handler.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/middlewares/base.py` & `aliceio-0.0.3/aliceio/dispatcher/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/middlewares/error.py` & `aliceio-0.0.3/aliceio/dispatcher/middlewares/error.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/middlewares/manager.py` & `aliceio-0.0.3/aliceio/dispatcher/middlewares/manager.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/middlewares/response_convert.py` & `aliceio-0.0.3/aliceio/dispatcher/middlewares/response_convert.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/dispatcher/middlewares/user_context.py` & `aliceio-0.0.3/aliceio/dispatcher/middlewares/user_context.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/enums/update.py` & `aliceio-0.0.3/aliceio/enums/update.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/filters/base.py` & `aliceio-0.0.3/aliceio/filters/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/filters/exception.py` & `aliceio-0.0.3/aliceio/filters/exception.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/filters/logic.py` & `aliceio-0.0.3/aliceio/filters/logic.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/filters/magic_data.py` & `aliceio-0.0.3/aliceio/filters/magic_data.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/filters/state.py` & `aliceio-0.0.3/aliceio/filters/state.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/context.py` & `aliceio-0.0.3/aliceio/fsm/context.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/state.py` & `aliceio-0.0.3/aliceio/fsm/state.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/strategy.py` & `aliceio-0.0.3/aliceio/fsm/strategy.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/middlewares/fsm_context.py` & `aliceio-0.0.3/aliceio/fsm/middlewares/fsm_context.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/storage/base.py` & `aliceio-0.0.3/aliceio/fsm/storage/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/storage/memory.py` & `aliceio-0.0.3/aliceio/fsm/storage/memory.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/fsm/storage/redis.py` & `aliceio-0.0.3/aliceio/fsm/storage/redis.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/handlers/__init__.py` & `aliceio-0.0.3/aliceio/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/handlers/base.py` & `aliceio-0.0.3/aliceio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/base.py` & `aliceio-0.0.3/aliceio/methods/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/images/delete_image.py` & `aliceio-0.0.3/aliceio/methods/images/delete_image.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/images/get_images.py` & `aliceio-0.0.3/aliceio/methods/images/get_images.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/images/upload_image.py` & `aliceio-0.0.3/aliceio/methods/images/upload_image.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/sounds/delete_sound.py` & `aliceio-0.0.3/aliceio/methods/sounds/delete_sound.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/sounds/get_sounds.py` & `aliceio-0.0.3/aliceio/methods/sounds/get_sounds.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/methods/sounds/upload_sound.py` & `aliceio-0.0.3/aliceio/methods/sounds/upload_sound.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/__init__.py` & `aliceio-0.0.3/aliceio/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/alice_event.py` & `aliceio-0.0.3/aliceio/types/alice_event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/alice_request.py` & `aliceio-0.0.3/aliceio/types/alice_request.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/alice_response.py` & `aliceio-0.0.3/aliceio/types/alice_response.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/analytic_event.py` & `aliceio-0.0.3/aliceio/types/analytic_event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/analytics.py` & `aliceio-0.0.3/aliceio/types/analytics.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/api_state.py` & `aliceio-0.0.3/aliceio/types/api_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from aliceio.types.base import AliceObject
 
 StateDict = Dict[str, Any]
 SessionState = StateDict
 UserState = StateDict
 ApplicationState = StateDict
@@ -12,24 +12,24 @@
 class ApiState(AliceObject):
     """
     Данные о сохранённом состоянии на стороне API Алисы.
 
     [Source](https://yandex.ru/dev/dialogs/alice/doc/request.html#request__state-desc)
     """
 
-    user: UserState
+    user: Optional[UserState] = None
     session: SessionState
     application: ApplicationState
 
     if TYPE_CHECKING:
 
         def __init__(
             __pydantic_self__,
             *,
-            user: UserState,
+            user: Optional[UserState] = None,
             session: SessionState,
             application: ApplicationState,
             **__pydantic_kwargs: Any,
         ) -> None:
             super().__init__(
                 session=session,
                 user=user,
```

### Comparing `aliceio-0.0.2/aliceio/types/application.py` & `aliceio-0.0.3/aliceio/types/application.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/audio_player.py` & `aliceio-0.0.3/aliceio/types/audio_player.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/audio_player_directive.py` & `aliceio-0.0.3/aliceio/types/audio_player_directive.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/audio_player_error.py` & `aliceio-0.0.3/aliceio/types/audio_player_error.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/audio_player_item.py` & `aliceio-0.0.3/aliceio/types/audio_player_item.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/base.py` & `aliceio-0.0.3/aliceio/types/base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/big_image.py` & `aliceio-0.0.3/aliceio/types/big_image.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/button_pressed.py` & `aliceio-0.0.3/aliceio/types/button_pressed.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/card_footer.py` & `aliceio-0.0.3/aliceio/types/card_footer.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/card_header.py` & `aliceio-0.0.3/aliceio/types/card_header.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/datetime.py` & `aliceio-0.0.3/aliceio/types/datetime.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/directives.py` & `aliceio-0.0.3/aliceio/types/directives.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/entity.py` & `aliceio-0.0.3/aliceio/types/entity.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/error_event.py` & `aliceio-0.0.3/aliceio/types/error_event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/error_result.py` & `aliceio-0.0.3/aliceio/types/error_result.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/fio_entity.py` & `aliceio-0.0.3/aliceio/types/fio_entity.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/geo_entity.py` & `aliceio-0.0.3/aliceio/types/geo_entity.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/image_gallery.py` & `aliceio-0.0.3/aliceio/types/image_gallery.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/image_gallery_item.py` & `aliceio-0.0.3/aliceio/types/image_gallery_item.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/input_file.py` & `aliceio-0.0.3/aliceio/types/input_file.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/interfaces.py` & `aliceio-0.0.3/aliceio/types/interfaces.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/item_image.py` & `aliceio-0.0.3/aliceio/types/item_image.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/items_list.py` & `aliceio-0.0.3/aliceio/types/items_list.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/markup.py` & `aliceio-0.0.3/aliceio/types/markup.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/media_button.py` & `aliceio-0.0.3/aliceio/types/media_button.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/message.py` & `aliceio-0.0.3/aliceio/types/message.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/meta.py` & `aliceio-0.0.3/aliceio/types/meta.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/metadata.py` & `aliceio-0.0.3/aliceio/types/metadata.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/nlu.py` & `aliceio-0.0.3/aliceio/types/nlu.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/purchase.py` & `aliceio-0.0.3/aliceio/types/purchase.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/quota.py` & `aliceio-0.0.3/aliceio/types/quota.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/response.py` & `aliceio-0.0.3/aliceio/types/response.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/result.py` & `aliceio-0.0.3/aliceio/types/result.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/session.py` & `aliceio-0.0.3/aliceio/types/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Optional
 
 from .application import Application
 from .base import AliceObject
 from .user import User
 
 
 class Session(AliceObject):
@@ -17,14 +17,15 @@
     skill_id: str
     # user_id: str  DEPRECATED. Use `Session.application.application_id`
     application: Application
     new: bool
     user: Optional[User] = None  # None если пользователь неавторизован
 
     if TYPE_CHECKING:
+        is_anonymous: ClassVar[bool]
 
         def __init__(
             __pydantic_self__,
             *,
             message_id: int,
             session_id: str,
             skill_id: str,
@@ -40,7 +41,13 @@
                 skill_id=skill_id,
                 # user_id=user_id,
                 user=user,
                 application=application,
                 new=new,
                 **__pydantic_kwargs,
             )
+
+    else:
+
+        @property
+        def is_anonymous(self) -> bool:
+            return self.user is None
```

### Comparing `aliceio-0.0.2/aliceio/types/show_item_meta.py` & `aliceio-0.0.3/aliceio/types/show_item_meta.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/show_pull.py` & `aliceio-0.0.3/aliceio/types/show_pull.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/space_status.py` & `aliceio-0.0.3/aliceio/types/space_status.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/stream.py` & `aliceio-0.0.3/aliceio/types/stream.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/text_button.py` & `aliceio-0.0.3/aliceio/types/text_button.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/timeout_event.py` & `aliceio-0.0.3/aliceio/types/timeout_event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/tokens_entity.py` & `aliceio-0.0.3/aliceio/types/tokens_entity.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/update.py` & `aliceio-0.0.3/aliceio/types/update.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/uploaded_image.py` & `aliceio-0.0.3/aliceio/types/uploaded_image.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/uploaded_sound.py` & `aliceio-0.0.3/aliceio/types/uploaded_sound.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/url.py` & `aliceio-0.0.3/aliceio/types/url.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/types/user.py` & `aliceio-0.0.3/aliceio/types/user.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/utils/builders.py` & `aliceio-0.0.3/aliceio/utils/builders.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/utils/funcs.py` & `aliceio-0.0.3/aliceio/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/utils/magic_filter.py` & `aliceio-0.0.3/aliceio/utils/magic_filter.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/utils/mixins.py` & `aliceio-0.0.3/aliceio/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/aliceio/webhook/aiohttp_server.py` & `aliceio-0.0.3/aliceio/webhook/aiohttp_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,17 +175,19 @@
     __call__ = handle
 
     # TODO: Проверить, помогает ли про запуске шоу Алисы
     @staticmethod
     def _convert_show_pull_to_normal_request(update: Dict[str, Any]) -> Dict[str, Any]:
         """
         При получении события запуска утреннего шоу вся информация
-        (мета, сессия, версия и реквест) находится по ключу body.
+        (мета, сессия, версия и реквест) вероятно находится по ключу body.
         Эта функция выносит всю информацию за это поле.
 
+        https://yandex.ru/dev/dialogs/alice/doc/request-show-pull.html
+
         :param update:
         :return:
         """
         return cast(Dict[str, Any], update.get("body", update))
 
     def _build_web_response(self, result: Any) -> web.Response:
         return web.Response(
```

### Comparing `aliceio-0.0.2/aliceio/webhook/security.py` & `aliceio-0.0.3/aliceio/webhook/security.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/index.md` & `aliceio-0.0.3/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Хаб
 
 Добро пожаловать в документацию AliceIO!
+Алисия - это асинхронный фреймворк на [python](https://www.python.org/){:target="_blank"},
+упрощающий разработку [навыков Алисы](https://dialogs.yandex.ru/store){:target="_blank"}
+из [Яндекс.Диалогов](https://dialogs.yandex.ru/development){:target="_blank"}.
 
 Начинающим рекомендуется ознакомиться с [туториалом](tutorial/index.md).
 Знание Python'а приветствуется и рекомендуется.
 
 > Проект написан с использованием исходного кода [aiogram](https://github.com/aiogram/aiogram/){:target="_blank"},
 > [vkbottle](https://github.com/vkbottle/vkbottle/){:target="_blank"}
 > и [aioalice](https://github.com/mahenzon/aioalice){:target="_blank"}
 >
-> Спасибо авторам и участникам этих замечательных библиотек
+> Спасибо авторам и участникам этих замечательных библиотек **<3**
```

### Comparing `aliceio-0.0.2/docs/_css/style.css` & `aliceio-0.0.3/docs/_css/style.css`

 * *Files 7% similar despite different names*

```diff
@@ -63,18 +63,14 @@
 
   .md-nav__title,
   .md-nav__link {
     box-shadow: none !important;
   }
 }
 
-.md-nav__item--section>.md-nav>.md-nav__list>.md-nav__item>.md-nav__link{
-  color: var(--md-typeset-a-color) !important;
-}
-
 @media screen and (max-width:76.1875em) {
   [data-md-color-scheme="slate"] .md-nav--primary .md-nav__title {
     background-color: var(--vkbottle-bg-darker);
   }
 }
 
 @media screen and (max-width: 59.9375em) {
```

### Comparing `aliceio-0.0.2/docs/_static/alice-skill.png` & `aliceio-0.0.3/docs/_static/alice-skill.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/create-dialog.png` & `aliceio-0.0.3/docs/_static/create-dialog.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/logo-aliceio-black-text.png` & `aliceio-0.0.3/docs/_static/logo-aliceio-black-text.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/logo-aliceio-black.png` & `aliceio-0.0.3/docs/_static/logo-aliceio-black.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/logo-aliceio-trans-text.png` & `aliceio-0.0.3/docs/_static/logo-aliceio-trans-text.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/logo-aliceio-trans.png` & `aliceio-0.0.3/docs/_static/logo-aliceio-trans.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/logo-aliceio-white-text.png` & `aliceio-0.0.3/docs/_static/logo-aliceio-white-text.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/logo-aliceio-white.png` & `aliceio-0.0.3/docs/_static/logo-aliceio-white.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/middleware-dark.png` & `aliceio-0.0.3/docs/_static/middleware-dark.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/middleware-light.png` & `aliceio-0.0.3/docs/_static/middleware-light.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/ngrok.png` & `aliceio-0.0.3/docs/_static/ngrok.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/save-settings.png` & `aliceio-0.0.3/docs/_static/save-settings.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/skill-id-url.png` & `aliceio-0.0.3/docs/_static/skill-id-url.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/skill-id.png` & `aliceio-0.0.3/docs/_static/skill-id.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/skill-settings.png` & `aliceio-0.0.3/docs/_static/skill-settings.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/_static/testing.png` & `aliceio-0.0.3/docs/_static/testing.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/dispatcher/flags.md` & `aliceio-0.0.3/docs/aliceio/dispatcher/flags.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/dispatcher/router.md` & `aliceio-0.0.3/docs/aliceio/dispatcher/router.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         - include_router
         - include_routers
 
 
 ## Наблюдатели
 
 !!! warning "Важно"
-    Все хэндлеры всегда должны быть асинхронными. Имя функции-обработчика не имеет значения.
-    Имя аргумента события также не важно, но рекомендуется не перекрывать имя контекстными данными, поскольку функция не может принимать два аргумента с одинаковым именем.
+    Все хэндлеры всегда должны быть асинхронными. Имя функции-обработчика не имеет значения. \
+    Имя аргумента события (первого аргумента) также не важно, но рекомендуется не перекрывать имя контекстными данными, поскольку функция не может принимать два аргумента с одинаковым именем.
 
 Вот список всех доступных наблюдателей и примеры регистрации хэндлеров.
 
 В этих примерах используется только регистрация через декоратор, но вы всегда можете использовать метод `<router>.<event_type>.register(...)`
 
 ### Сообщение (SimpleUtterance)
 ```python
@@ -52,24 +52,24 @@
 ## Вложенные роутеры
 
 Событие будет распространять по роутерам и хэндлерам согласно порядку их добавления.
 
 !!! warning "Важно"
     Роутеры могут быть включены в другие роутеры с некоторыми ограничениями:
 
-    1. Роутер не может подключить сам себя
-    2. Роутеры не могут составлять цикл (р1 содержит р2, р2 содержит р3, р3 содерит р1)
+    1. Роутер не может подключить сам себя.
+    2. Роутеры не могут составлять цикл (р1 содержит р2, р2 содержит р3, р3 содерит р1).
 
 ## Update
 ```python
 @dispatcher.update()
 async def update_handler(update: Update) -> Any: pass
 ```
 
-!!! warning "Предупреждение"
+!!! warning "Важно"
     Только диспетчер может обрабатывать события с типом `Update`.
 
 !!! note "Примечание"
     В диспетчере уже есть обработчик этого типа событий, поэтому вы можете использовать его для обработки всех обновлений, которые не обработались другими хэндлерами.
 
 
 ## Источники
```

### Comparing `aliceio-0.0.2/docs/aliceio/enums/all-enums.md` & `aliceio-0.0.3/docs/aliceio/enums/all-enums.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/filters/base.md` & `aliceio-0.0.3/docs/aliceio/filters/base.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/filters/magic-filter.md` & `aliceio-0.0.3/docs/aliceio/filters/magic-filter.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/types/uploaded-sound.md` & `aliceio-0.0.3/docs/aliceio/types/uploaded-sound.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/utils/builders.md` & `aliceio-0.0.3/docs/aliceio/utils/builders.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/webhook/aiohttp-server.md` & `aliceio-0.0.3/docs/aliceio/webhook/aiohttp-server.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/aliceio/webhook/security.md` & `aliceio-0.0.3/docs/aliceio/webhook/security.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/templates/python/material/languages/en.html` & `aliceio-0.0.3/docs/templates/python/material/languages/en.html`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/dependency-injection.md` & `aliceio-0.0.3/docs/tutorial/dependency-injection.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/error-handling.md` & `aliceio-0.0.3/docs/tutorial/error-handling.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/filters.md` & `aliceio-0.0.3/docs/tutorial/filters.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/finite-state-machine.md` & `aliceio-0.0.3/docs/tutorial/finite-state-machine.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,23 @@
 
     return Response(text="Окей, стою. Пока-пока!", end_session=True)
 ```
 
 Готово!
 
 !!! warning "Важно"
-    Вероятно, в навыках в черновиках не работают состояния на стороне Алисы. Используйте MemoryStorage для тестирования.
+    Чтобы использовать хранилище на стороне Алисы, включите его в настройках навыка.
+
+    ![alice-storage.png](../_static/alice-storage.png)
+
+!!! note "Примечание"
+    Если навыком пользуется неавторизованный пользователь, то FSMStrategy.USER будет как FSMStrategy.APPLICATION:
+
+    - для локальных хранилищ user_id будет равен application_id
+    - в хранилище на стороне Алисы состояние будет храниться по устройству
+
 
 ## Примеры
 
 * [fsm_form](https://github.com/K1rL3s/aliceio/blob/master/examples/fsm_form.py){:target="_blank"}
 * [fsm_games](https://github.com/K1rL3s/aliceio/blob/master/examples/fsm_games.py){:target="_blank"}
 * [aiogram](https://docs.aiogram.dev/en/dev-3.x/dispatcher/finite_state_machine/index.html){:target="_blank"}
```

### Comparing `aliceio-0.0.2/docs/tutorial/first-skill.md` & `aliceio-0.0.3/docs/tutorial/first-skill.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/full-skill.md` & `aliceio-0.0.3/docs/tutorial/full-skill.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/index.md` & `aliceio-0.0.3/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/methods.md` & `aliceio-0.0.3/docs/tutorial/methods.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Чтобы получить, загрузить и удалить загруженные изображения и звуки, надо передать [OAuth Token](https://yandex.ru/dev/direct/doc/start/token.html){:target="_blank"} при создании навыка и воспользоваться одним из следующих методов экземпляра:
 
 ```python
 skill = Skill(skill_id="...", oauth_token="it_is_required_for_methods")
 ```
 
-!!! warning "Предупреждение"
+!!! warning "Важно"
     Без токена невозможно использовать все следующие методы.
 
 ## Свободное место
 
 ### ::: aliceio.client.skill.Skill.status
     handler: python
     options:
```

### Comparing `aliceio-0.0.2/docs/tutorial/middlewares.md` & `aliceio-0.0.3/docs/tutorial/middlewares.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/routers.md` & `aliceio-0.0.3/docs/tutorial/routers.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Роутеры
 
 Далее в туториале регистрация хэндлеров будет происходить через роутеры.
-Подробнее про них и существующие события Алисы можно узнать [здесь](../aliceio/dispatcher/router.md). \
+Подробнее про них и существующие события Алисы можно узнать [здесь](../aliceio/dispatcher/router.md){:target="_blank"}.
+
 Роутеры нужны для разделения проекта на несколько файлов и гибкой установки мидлварей и фильтров, но об этом подробнее к концу гайда.
 
 !!! note "Примечание"
     Диспетчер - тоже роутер.
 
 ## Примеры
```

### Comparing `aliceio-0.0.2/docs/tutorial/special-events.md` & `aliceio-0.0.3/docs/tutorial/special-events.md`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/docs/tutorial/start.md` & `aliceio-0.0.3/docs/tutorial/start.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
     Чтобы провести первый запуск, нужно подключить вебхук к Диалогам. \
     Его можно сделать через [ngrok](https://ngrok.com/){:target="_blank"} - это сервис, который позволяет сделать локальный порт доступным из интернета без настройки NAT, роутера, DDNS и других протоколов.
     Программа создает туннель между вашим компьютером и удалённым сервером и предоставляет доступ к нему с уникального домена.
 
     1. [Установите](https://dashboard.ngrok.com/get-started/setup){:target="_blank"}, разархивируйте и запустите ngrok.
     2. Добавьте ваш [auth-token](https://dashboard.ngrok.com/get-started/your-authtoken){:target="_blank"} в консоль ngrok'а.
-        ```console
+        ```bash
         ngrok config add-authtoken <your-token-here>
         ```
     3. Запустите ngrok
-        ```console
+        ```bash
         ngrok http 80
         ```
     4. Через пару секунд появится длинная ссылка. Её надо указать как вебхук юрл и добавить **/alice** после ссылки:
 
-        !!! warning ""Важно"
+        !!! warning "Важно"
             Не выключайте ngrok, иначе туннель закроется.
 
         ![ngrok.png](../_static/ngrok.png)
 
         ![skill-settings.png](../_static/skill-settings.png)
 
 6. Сохраните изменения внизу страницы.
@@ -53,19 +53,29 @@
 
 Или в ссылке в поисковой строке:
 
 ![skill-id-url.png](../_static/skill-id-url.png)
 
 
 !!! note "Примечание"
-    Для запуска в прод вам нужен свой домен и SSL сертификат, об этом подробнее в [официальной документации](https://yandex.ru/dev/dialogs/alice/doc/deploy-overview.html){:target="_blank"}.
+    Для запуска в прод вам нужен свой домен и [SSL сертификат](https://wiki.yaboard.com/s/zc){:target="_blank"},
+    об этом подробнее в [официальной документации](https://yandex.ru/dev/dialogs/alice/doc/deploy-overview.html){:target="_blank"}.
 
 
 ## [Код](https://github.com/K1rL3s/aliceio/blob/master/examples/fast_start.py){:target="_blank"}
 
+> Если вы ещё не установили библиотеку, то это можно сделать так:
+> ```bash
+> pip install -U aliceio
+> ```
+> Или:
+> ```bash
+> python -m pip install -U aliceio
+> ```
+
 Самый простой навык, который умеет только приветствовать пользователя. \
 Скопируйте его, укажите айди вашего навыка и запустите скрипт.
 
 ```python
 from aiohttp import web
 from aliceio import Dispatcher, Skill
 from aliceio.types import Message
```

### Comparing `aliceio-0.0.2/examples/builders.py` & `aliceio-0.0.3/examples/builders.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/buy_elephant.py` & `aliceio-0.0.3/examples/buy_elephant.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/context_addition.py` & `aliceio-0.0.3/examples/context_addition.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/echo_skill.py` & `aliceio-0.0.3/examples/echo_skill.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/echo_skill_ssl.py` & `aliceio-0.0.3/examples/echo_skill_ssl.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/error_handling.py` & `aliceio-0.0.3/examples/error_handling.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/fast_start.py` & `aliceio-0.0.3/examples/fast_start.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/filters.py` & `aliceio-0.0.3/examples/filters.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/fsm_form.py` & `aliceio-0.0.3/examples/fsm_form.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,17 +102,17 @@
         if positive
         else "тебе не нравятся навыки Алисы..."
     )
     return text
 
 
 def main() -> None:
-    # use_api_storage можно и на False,
-    # тогда будет использоваться хранилище на текущей машине
-    dp = Dispatcher(use_api_storage=True, response_timeout=10**9)
+    # use_api_storage можно и на True,
+    # тогда будет использоваться хранилище на стороне Алисы
+    dp = Dispatcher(use_api_storage=False)
     dp.include_router(form_router)
 
     skill_id = os.environ["SKILL_ID"]
     skill = Skill(skill_id=skill_id)
 
     app = web.Application()
     webhook_requests_handler = OneSkillRequestHandler(
```

### Comparing `aliceio-0.0.2/examples/fsm_games.py` & `aliceio-0.0.3/examples/fsm_games.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import random
-from typing import List, Sequence
+from typing import Any, Dict, List, Sequence, cast
 
 from aiohttp import web
 
 from aliceio import Dispatcher, F, Router, Skill
 from aliceio.filters import BaseFilter
 from aliceio.fsm.context import FSMContext
 from aliceio.fsm.state import State, StatesGroup
@@ -125,15 +125,15 @@
         buttons=generate_thimbles(),
     )
 
 
 # Создаёт три напёрстка, среди которых один выигрышный
 def generate_thimbles() -> List[TextButton]:
     buttons = [TextButton(title=THIMBLE, payload={"win": False}) for _ in range(3)]
-    random.choice(buttons).payload["win"] = True
+    cast(Dict[str, Any], random.choice(buttons).payload)["win"] = True
     return buttons
 
 
 # Обработка всех остальных случаев, которые не обработались выше
 @router.message()
 @router.button_pressed()
 async def wtf_is_happened(event: AliceEvent, state: FSMContext) -> Response:
@@ -141,16 +141,18 @@
     await state.set_state(Game.select)
     return Response(
         text="Не понял тебя. Давай сначала.",
         buttons=[TextButton(title=title.capitalize()) for title in GAMES_LIST],
     )
 
 
-def main():
-    dp = Dispatcher()
+def main() -> None:
+    # use_api_storage можно и на True,
+    # тогда будет использоваться хранилище на стороне Алисы
+    dp = Dispatcher(use_api_storage=False)
     dp.include_router(router)
 
     skill_id = os.environ["SKILL_ID"]
     skill = Skill(skill_id=skill_id)
 
     app = web.Application()
     webhook_requests_handler = OneSkillRequestHandler(
```

### Comparing `aliceio-0.0.2/examples/methods.py` & `aliceio-0.0.3/examples/methods.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/middlewares.py` & `aliceio-0.0.3/examples/middlewares.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/special_events.py` & `aliceio-0.0.3/examples/special_events.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/data/watermelon.png` & `aliceio-0.0.3/examples/data/watermelon.png`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/data/watermelon_rip.mp3` & `aliceio-0.0.3/examples/data/watermelon_rip.mp3`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/data/watermelon_rip2.mp3` & `aliceio-0.0.3/examples/data/watermelon_rip2.mp3`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/examples/multi_file_skill/skill.py` & `aliceio-0.0.3/examples/multi_file_skill/skill.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/conftest.py` & `aliceio-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/mocked/mocked_skill.py` & `aliceio-0.0.3/tests/mocked/mocked_skill.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/mocked/mocked_update.py` & `aliceio-0.0.3/tests/mocked/mocked_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, List, Optional
 
+from aliceio import __api_version__
 from aliceio.enums.entity import EntityType
 from aliceio.enums.update import RequestType
 from aliceio.types import (
     NLU,
     AliceRequest,
     ApiState,
     Application,
@@ -63,15 +64,15 @@
     )
     state = create_mocked_api_state(state, user_state, session_state, application_state)
 
     return Update(
         meta=meta,
         session=session,
         request=request,
-        version="1.0",
+        version=__api_version__,
         context={"skill": skill} if skill else None,
         state=state,
     )
 
 
 def create_mocked_meta(
     meta: Optional[Meta] = None,
```

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_alice_server.py` & `aliceio-0.0.3/tests/test_api/test_client/test_alice_server.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_context_controller.py` & `aliceio-0.0.3/tests/test_api/test_client/test_context_controller.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_skill.py` & `aliceio-0.0.3/tests/test_api/test_client/test_skill.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_session/test_aiohttp_session.py` & `aliceio-0.0.3/tests/test_api/test_client/test_session/test_aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_session/test_base_session.py` & `aliceio-0.0.3/tests/test_api/test_client/test_session/test_base_session.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_session/test_middlewares/test_manager.py` & `aliceio-0.0.3/tests/test_api/test_client/test_session/test_middlewares/test_manager.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_client/test_session/test_middlewares/test_request_logging.py` & `aliceio-0.0.3/tests/test_api/test_client/test_session/test_middlewares/test_request_logging.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_audio_player_directive.py` & `aliceio-0.0.3/tests/test_api/test_types/test_audio_player_directive.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_card.py` & `aliceio-0.0.3/tests/test_api/test_types/test_card.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_entity.py` & `aliceio-0.0.3/tests/test_api/test_types/test_entity.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_input_file.py` & `aliceio-0.0.3/tests/test_api/test_types/test_input_file.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_message.py` & `aliceio-0.0.3/tests/test_api/test_types/test_message.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_timeout_event.py` & `aliceio-0.0.3/tests/test_api/test_types/test_timeout_event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_update.py` & `aliceio-0.0.3/tests/test_api/test_types/test_update.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_api/test_types/test_uploaded.py` & `aliceio-0.0.3/tests/test_api/test_types/test_uploaded.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_dispatcher.py` & `aliceio-0.0.3/tests/test_dispatcher/test_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,39 +228,39 @@
         class MyStorage(MemoryStorage):
             pass
 
         dp = Dispatcher()
         my_storage = MyStorage()
 
         assert (
-            dp._init_storage(my_storage, disable_fsm=False, use_api_storage=False)
+            dp._create_storage(my_storage, disable_fsm=False, use_api_storage=False)
             == my_storage
         )
         assert (
-            dp._init_storage(my_storage, disable_fsm=False, use_api_storage=True)
+            dp._create_storage(my_storage, disable_fsm=False, use_api_storage=True)
             == my_storage
         )
         assert (
-            dp._init_storage(my_storage, disable_fsm=True, use_api_storage=False)
+            dp._create_storage(my_storage, disable_fsm=True, use_api_storage=False)
             == my_storage
         )
         assert (
-            dp._init_storage(my_storage, disable_fsm=True, use_api_storage=True)
+            dp._create_storage(my_storage, disable_fsm=True, use_api_storage=True)
             == my_storage
         )
 
         assert isinstance(
-            dp._init_storage(None, disable_fsm=False, use_api_storage=False),
+            dp._create_storage(None, disable_fsm=False, use_api_storage=False),
             MemoryStorage,
         )
         assert isinstance(
-            dp._init_storage(None, disable_fsm=False, use_api_storage=True),
+            dp._create_storage(None, disable_fsm=False, use_api_storage=True),
             ApiStorage,
         )
         assert isinstance(
-            dp._init_storage(None, disable_fsm=True, use_api_storage=False),
+            dp._create_storage(None, disable_fsm=True, use_api_storage=False),
             MemoryStorage,
         )
         assert isinstance(
-            dp._init_storage(None, disable_fsm=True, use_api_storage=True),
+            dp._create_storage(None, disable_fsm=True, use_api_storage=True),
             MemoryStorage,
         )
```

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_router.py` & `aliceio-0.0.3/tests/test_dispatcher/test_router.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_timeout.py` & `aliceio-0.0.3/tests/test_dispatcher/test_timeout.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_event/test_alice.py` & `aliceio-0.0.3/tests/test_dispatcher/test_event/test_alice.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_event/test_event.py` & `aliceio-0.0.3/tests/test_dispatcher/test_event/test_event.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_event/test_handler.py` & `aliceio-0.0.3/tests/test_dispatcher/test_event/test_handler.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_event/test_middleware.py` & `aliceio-0.0.3/tests/test_dispatcher/test_event/test_middleware.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_middlewares/test_error.py` & `aliceio-0.0.3/tests/test_dispatcher/test_middlewares/test_error.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_middlewares/test_response_converter.py` & `aliceio-0.0.3/tests/test_dispatcher/test_middlewares/test_response_converter.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_dispatcher/test_middlewares/test_user_context.py` & `aliceio-0.0.3/tests/test_dispatcher/test_middlewares/test_user_context.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_filters/test_base.py` & `aliceio-0.0.3/tests/test_filters/test_base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_filters/test_exception.py` & `aliceio-0.0.3/tests/test_filters/test_exception.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_filters/test_logic.py` & `aliceio-0.0.3/tests/test_filters/test_logic.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_filters/test_magic_data.py` & `aliceio-0.0.3/tests/test_filters/test_magic_data.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_filters/test_state.py` & `aliceio-0.0.3/tests/test_filters/test_state.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_flags/test_decorator.py` & `aliceio-0.0.3/tests/test_flags/test_decorator.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_flags/test_getter.py` & `aliceio-0.0.3/tests/test_flags/test_getter.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_fsm/test_context.py` & `aliceio-0.0.3/tests/test_fsm/test_context.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_fsm/test_state.py` & `aliceio-0.0.3/tests/test_fsm/test_state.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_fsm/test_strategy.py` & `aliceio-0.0.3/tests/test_fsm/test_strategy.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_fsm/middlewares/test_api_storage.py` & `aliceio-0.0.3/tests/test_fsm/middlewares/test_api_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,25 @@
                     session={},
                     application={
                         "state": FSMStrategy.APPLICATION,
                         "data": {"foo": "bar"},
                     },
                 ),
             ],
+            [
+                FSMStrategy.USER,
+                ApiState(
+                    user=None,
+                    session={},
+                    application={
+                        "state": FSMStrategy.USER,
+                        "data": {"foo": "bar"},
+                    },
+                ),
+            ],
         ],
     )
     async def test_resolve_state_data(
         self,
         strategy: FSMStrategy,
         api_state: ApiState,
     ):
@@ -97,47 +108,43 @@
         middleware = FSMApiStorageMiddleware(strategy=strategy)
 
         record = middleware.resolve_state_data(api_state)
 
         assert record.state == FSMStrategy.SESSION
         assert record.data == {"sess": "ion"}
 
-    # В навыках в черновиках, вероятно, не работают состояния на стороне Алисы
     async def test_resolve_state_none(self):
         middleware = FSMApiStorageMiddleware(strategy=None)
 
         record = middleware.resolve_state_data(None)
 
         assert record.state is None
         assert record.data == {}
 
-    async def test_pre_set_state_no_data(self, state: FSMContext, update: Update):
+    async def test_state_from_alice_no_data(self, state: FSMContext, update: Update):
         for strategy in (
             FSMStrategy.USER,
             FSMStrategy.SESSION,
             FSMStrategy.APPLICATION,
         ):
             middleware = FSMApiStorageMiddleware(strategy=strategy)
-            await middleware.pre_set_state(update, state)
+            await middleware.set_state_from_alice(update, state)
             assert await state.get_state() is None
             assert await state.get_data() == {}
 
-    async def test_pre_set_state_data_and_strategy(
-        self,
-        state: FSMContext,
-    ):
+    async def test_state_from_alice_data_and_strategy(self, state: FSMContext):
         update = create_mocked_update(
             user_state={"state": "MyState", "data": {"foo": "bar"}}
         )
         middleware = FSMApiStorageMiddleware(strategy=FSMStrategy.USER)
 
         assert await state.get_state() is None
         assert await state.get_data() == {}
 
-        await middleware.pre_set_state(update, state)
+        await middleware.set_state_from_alice(update, state)
 
         assert await state.get_state() == "MyState"
         assert await state.get_data() == {"foo": "bar"}
 
     @pytest.mark.parametrize(
         "strategy,state_attr,new_state",
         [
@@ -203,41 +210,57 @@
 
         middleware.set_new_state(response, new_state)
 
         assert getattr(response, state_attr) == new_state
         for attr in state_attrs:
             assert getattr(response, attr) is None
 
-    async def test_post_update(self, state: FSMContext):
+    async def test_set_new_state_with_anonymous_user(self, state: FSMContext):
+        middleware = FSMApiStorageMiddleware(strategy=FSMStrategy.USER)
+        response = AliceResponse(response=Response(text="test"))
+        new_state = {"state": "session", "data": {"foo": "bar"}}
+
+        state_attrs = ["user_state_update", "session_state", "application_state"]
+        for attr in state_attrs:
+            assert getattr(response, attr) is None
+        state_attrs.remove("application_state")
+
+        middleware.set_new_state(response, new_state, is_anonymous=True)
+
+        assert response.application_state == new_state
+        for attr in state_attrs:
+            assert getattr(response, attr) is None
+
+    async def test_set_state_to_alice(self, state: FSMContext):
         middleware = FSMApiStorageMiddleware(strategy=FSMStrategy.USER)
         result = AliceResponse(response=Response(text="test"))
         await state.set_state("MyState")
         await state.set_data({"foo": "bar"})
         await state.update_data(bar="foo")
 
         assert result.user_state_update is None
 
-        await middleware.post_update_state(result, state)
+        await middleware.set_state_to_alice(result, state)
 
         assert result.user_state_update == {
             "state": "MyState",
             "data": {"foo": "bar", "bar": "foo"},
         }
         assert await state.get_state() == "MyState"
         assert await state.get_data() == {"foo": "bar", "bar": "foo"}  # нет очистки
 
-    async def test_post_update_empty_context(self, state: FSMContext):
+    async def test_set_state_to_alice_empty_context(self, state: FSMContext):
         middleware = FSMApiStorageMiddleware(strategy=FSMStrategy.USER)
         result = AliceResponse(response=Response(text="test"))
 
         assert result.user_state_update is None
         assert result.session_state is None
         assert result.application_state is None
 
-        await middleware.post_update_state(result, state)
+        await middleware.set_state_to_alice(result, state)
 
         assert result.user_state_update == {"state": None, "data": {}}
         assert result.session_state is None
         assert result.application_state is None
         assert await state.get_state() is None
         assert await state.get_data() == {}
```

### Comparing `aliceio-0.0.2/tests/test_fsm/middlewares/test_fsm_context.py` & `aliceio-0.0.3/tests/test_fsm/middlewares/test_fsm_context.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_fsm/storage/test_redis.py` & `aliceio-0.0.3/tests/test_fsm/storage/test_redis.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_fsm/storage/test_storages.py` & `aliceio-0.0.3/tests/test_fsm/storage/test_storages.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_audio_player.py` & `aliceio-0.0.3/tests/test_handlers/test_audio_player.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_base.py` & `aliceio-0.0.3/tests/test_handlers/test_base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_button_pressed.py` & `aliceio-0.0.3/tests/test_handlers/test_button_pressed.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_message.py` & `aliceio-0.0.3/tests/test_handlers/test_message.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_purchase.py` & `aliceio-0.0.3/tests/test_handlers/test_purchase.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_show_pull.py` & `aliceio-0.0.3/tests/test_handlers/test_show_pull.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_handlers/test_timeout.py` & `aliceio-0.0.3/tests/test_handlers/test_timeout.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_methods/test_base.py` & `aliceio-0.0.3/tests/test_methods/test_base.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_methods/test_images.py` & `aliceio-0.0.3/tests/test_methods/test_images.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_methods/test_sounds.py` & `aliceio-0.0.3/tests/test_methods/test_sounds.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_utils/test_builders.py` & `aliceio-0.0.3/tests/test_utils/test_builders.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_utils/test_exceptions.py` & `aliceio-0.0.3/tests/test_utils/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_utils/test_magic_filter.py` & `aliceio-0.0.3/tests/test_utils/test_magic_filter.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_utils/test_mixins.py` & `aliceio-0.0.3/tests/test_utils/test_mixins.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/tests/test_webhook/test_aiohttp_server.py` & `aliceio-0.0.3/tests/test_webhook/test_aiohttp_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from typing import Awaitable, Callable
 
 import pytest
 from aiohttp import web
 from aiohttp.test_utils import TestClient
 from aiohttp.web_app import Application
 
@@ -221,29 +220,34 @@
                 EventType.SHOW_PULL,
                 '{"meta": {"locale": "ru-RU", "timezone": "Europe/Moscow", "client_id": "ru.yandex.searchplugin/7.16 (none none; android 4.4.2)", "interfaces": {"screen": {}, "account_linking": {}, "audio_player": {}}}, "request": {"type": "Show.Pull", "show_type": "MORNING"}, "session": {"message_id": 0, "session_id": "42:SESSION_ID", "skill_id": "42:SKILL_ID", "user_id": "42:DEPRECATED_USER_ID", "user": {"user_id": "42:USER_ID", "access_token": "42:ACCESS_TOKEN"}, "application": {"application_id": "42:APP_ID"}, "new": false}, "state": {"session": {"value": 10}, "user": {"value": 42}, "application": {"value": 37}}, "version": "1.0"}',  # noqa: E501
             ],
             [
                 EventType.MESSAGE,
                 '{"meta": {"locale": "ru-RU", "timezone": "Europe/Moscow", "client_id": "ru.yandex.searchplugin/7.16 (none none; android 4.4.2)", "interfaces": {"screen": {}, "account_linking": {}, "audio_player": {}}}, "request": {"command": "закажи пиццу на улицу льва толстого 16 на завтра", "original_utterance": "закажи пиццу на улицу льва толстого, 16 на завтра", "markup": {"dangerous_context": true}, "payload": {}, "nlu": {"tokens": ["закажи", "пиццу", "на", "льва", "толстого", "16", "на", "завтра"], "entities": [{"tokens": {"start": 2, "end": 6}, "type": "YANDEX.GEO", "value": {"house_number": "16", "street": "льва толстого"}}, {"tokens": {"start": 3, "end": 5}, "type": "YANDEX.FIO", "value": {"first_name": "лев", "last_name": "толстой"}}, {"tokens": {"start": 5, "end": 6}, "type": "YANDEX.NUMBER", "value": 16}, {"tokens": {"start": 6, "end": 8}, "type": "YANDEX.DATETIME", "value": {"day": 1, "day_is_relative": true}}], "intents": {}}, "type": "SimpleUtterance"}, "session": {"message_id": 0, "session_id": "42:SESSION_ID", "skill_id": "42:SKILL_ID", "user_id": "42:DEPRECATED_USER_ID", "user": {"user_id": "42:USER_ID", "access_token": "42:ACCESS_TOKEN"}, "application": {"application_id": "42:APP_ID"}, "new": false}, "state": {"session": {"value": 10}, "user": {"value": 42}, "application": {"value": 37}}, "version": "1.0"}',  # noqa: E501
             ],
+            [
+                # Запрос от анонимного пользователя
+                EventType.MESSAGE,
+                '{"meta": {"locale": "ru-RU", "timezone": "Europe/Moscow", "client_id": "ru.yandex.searchplugin/7.16 (none none; android 4.4.2)", "interfaces": {"screen": {}, "account_linking": {}, "audio_player": {}}}, "request": {"command": "закажи пиццу на улицу льва толстого 16 на завтра", "original_utterance": "закажи пиццу на улицу льва толстого, 16 на завтра", "markup": {"dangerous_context": true}, "payload": {}, "nlu": {"tokens": ["закажи", "пиццу", "на", "льва", "толстого", "16", "на", "завтра"], "entities": [{"tokens": {"start": 2, "end": 6}, "type": "YANDEX.GEO", "value": {"house_number": "16", "street": "льва толстого"}}, {"tokens": {"start": 3, "end": 5}, "type": "YANDEX.FIO", "value": {"first_name": "лев", "last_name": "толстой"}}, {"tokens": {"start": 5, "end": 6}, "type": "YANDEX.NUMBER", "value": 16}, {"tokens": {"start": 6, "end": 8}, "type": "YANDEX.DATETIME", "value": {"day": 1, "day_is_relative": true}}], "intents": {}}, "type": "SimpleUtterance"}, "session": {"message_id": 0, "session_id": "42:SESSION_ID", "skill_id": "42:SKILL_ID", "user_id": "42:DEPRECATED_USER_ID", "application": {"application_id": "42:APP_ID"}, "new": false}, "state": {"session": {"value": 10}, "application": {"value": 37}}, "version": "1.0"}',  # noqa: E501
+            ],
         ],
     )
     async def test_feed_webhook_update(
         self,
         event_type: str,
         update: str,
         skill: MockedSkill,
         aiohttp_client: Callable[..., Awaitable[TestClient]],
     ):
         async def fn_handler(
-            event, skill, event_update, event_from_user, event_session
+            event, skill, event_update, event_session, event_from_user=None
         ):
             assert isinstance(skill, MockedSkill)
             assert isinstance(event_update, Update)
-            assert isinstance(event_from_user, User)
+            assert isinstance(event_from_user, User) or event_from_user is None
             assert isinstance(event_session, Session)
             assert event_update.event == event
             assert event_update.skill is event.skill is skill
             assert event.user == event_from_user
             assert event.session == event_session
             return "Handled"
```

### Comparing `aliceio-0.0.2/tests/test_webhook/test_security.py` & `aliceio-0.0.3/tests/test_webhook/test_security.py`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/.gitignore` & `aliceio-0.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -118,9 +118,8 @@
 00000750: 5465 7374 2064 6174 6162 6173 6573 0d0a  Test databases..
 00000760: 2a2e 6462 0d0a 2e64 620d 0a2a 2e64 622d  *.db...db..*.db-
 00000770: 7368 6d0d 0a2a 2e64 622d 7761 6c0d 0a0d  shm..*.db-wal...
 00000780: 0a23 2050 7974 6573 740d 0a2e 7079 7465  .# Pytest...pyte
 00000790: 7374 5f63 6163 6865 0d0a 0d0a 2e76 7363  st_cache.....vsc
 000007a0: 6f64 650d 0a2e 7669 6d0d 0a0d 0a23 2052  ode...vim....# R
 000007b0: 7566 660d 0a2e 7275 6666 5f63 6163 6865  uff...ruff_cache
-000007c0: 7300 6900 7400 6500 2f00 0d0a 000d 0a00  s.i.t.e./.......
-000007d0: 0d0a                                     ..
+000007c0: 0d0a                                     ..
```

### Comparing `aliceio-0.0.2/LICENSE` & `aliceio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/README.md` & `aliceio-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,29 @@
     <img width="200px" height="200px" alt="aliceio" src="https://raw.githubusercontent.com/K1rL3s/aliceio/master/docs/_static/logo-aliceio-trans-text.png">
   </a>
 </p>
 <h1 align="center">
   AliceIO
 </h1>
 
-<p align="center">
-  <img alt="License" src="https://img.shields.io/pypi/l/aliceio.svg?style=flat-square">
-  <img alt="Status" src="https://img.shields.io/pypi/status/aliceio.svg?style=flat-square">
-  <img alt="PyPI" src="https://img.shields.io/pypi/v/aliceio?label=pypi&style=flat-square">
-  <img alt="Downloads" src="https://img.shields.io/pypi/dw/aliceio.svg?style=flat-square">
-  <img alt="Supported python versions" src="https://img.shields.io/pypi/pyversions/aliceio.svg?style=flat-square">
-  <img alt="Tests" src="https://img.shields.io/github/actions/workflow/status/K1rL3s/aliceio/tests.yml?style=flat-square">
-</p>
+<div align="center">
+
+[![License](https://img.shields.io/pypi/l/aliceio.svg?style=flat)](https://github.com/K1rL3s/aliceio/blob/master/LICENSE)
+[![Status](https://img.shields.io/pypi/status/aliceio.svg?style=flat)](https://pypi.org/project/aliceio/)
+[![PyPI](https://img.shields.io/pypi/v/aliceio?label=pypi&style=flat)](https://pypi.org/project/aliceio/)
+[![Downloads](https://img.shields.io/pypi/dm/aliceio.svg?style=flat)](https://pypi.org/project/aliceio/)
+[![GitHub Repo stars](https://img.shields.io/github/stars/K1rL3s/aliceio?style=flat)](https://github.com/K1rL3s/aliceio/stargazers)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/aliceio.svg?style=flat)](https://pypi.org/project/aliceio/)
+[![Tests](https://img.shields.io/github/actions/workflow/status/K1rL3s/aliceio/tests.yml?style=flat)](https://github.com/K1rL3s/aliceio/actions)
+[![Coverage](https://codecov.io/gh/K1rL3s/aliceio/graph/badge.svg?style=flat)](https://codecov.io/gh/K1rL3s/aliceio)
+
+</div>
 <p align="center">
     <b>
-        Асинхронный фреймворк для
+        Асинхронный фреймворк, упрощающий разработку
         <a target="_blank" href="https://dialogs.yandex.ru/store">навыков Алисы</a>
         из
         <a target="_blank" href="https://dialogs.yandex.ru/development">Яндекс.Диалогов</a>
     </b>
 </p>
 <p align="center">
     Based on <a target="_blank" href="https://github.com/aiogram/aiogram/tree/dev-3.x">aiogram v3</a>
@@ -35,15 +39,15 @@
 - Машина состояний (Finite State Machine)
 - Мидлвари (для входящих событий и вызовов API)
 - Мощные [магические фильтры](https://github.com/aiogram/magic-filter)
 - Реакция на [долгое время работы](https://yandex.ru/dev/dialogs/alice/doc/publish-settings.html#troubleshooting)
 
 
 ### Важно!
-Настоятельно рекомендуется иметь опыт работы с [asyncio](https://docs.python.org/3/library/asyncio.html) перед использование **aliceio**
+Настоятельно рекомендуется иметь опыт работы с [asyncio](https://docs.python.org/3/library/asyncio.html) перед использованием **aliceio**
 
 
 ## Быстрый старт
 
 Как получить `skill_id` и подключить навык к Алисе можно прочитать <a target="_blank" href="https://aliceio.readthedocs.io/ru/latest/tutorial/start/">тут</a>.
 
 ```python
@@ -79,13 +83,13 @@
 - [Туториал](https://aliceio.readthedocs.io/ru/latest/tutorial/start/)
 - [Документация](https://aliceio.readthedocs.io/)
 - [Примеры](https://github.com/K1rL3s/aliceio/tree/master/examples)
 
 
 ## Связь
 Если у вас есть вопросы, вы можете посетить чат сообщества в Telegram
--   🇷🇺 [\@aliceio_ru](https://t.me/aliceio_ru)
+-   🇷🇺 [\@aliceio_chat](https://t.me/aliceio_chat)
 
 
 ## Лицензия
 Copyright © 2023-2024 [K1rL3s](https://github.com/K1rL3s) and [ZloyKobra](https://github.com/ZloyKobra) \
 Этот проект использует [MIT](https://github.com/K1rL3s/aliceio/blob/master/LICENSE) лицензию
```

### Comparing `aliceio-0.0.2/pyproject.toml` & `aliceio-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aliceio-0.0.2/PKG-INFO` & `aliceio-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aliceio
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous framework for Alice from Yandex Dialogs
 Project-URL: Documentation, https://aliceio.rtfd.io
 Project-URL: Repository, https://github.com/K1rL3s/aliceio
 Author: K1rL3s - Kirill Lesovoy
 Maintainer: K1rL3s - Kirill Lesovoy
 License: MIT License
         
@@ -91,25 +91,29 @@
     <img width="200px" height="200px" alt="aliceio" src="https://raw.githubusercontent.com/K1rL3s/aliceio/master/docs/_static/logo-aliceio-trans-text.png">
   </a>
 </p>
 <h1 align="center">
   AliceIO
 </h1>
 
-<p align="center">
-  <img alt="License" src="https://img.shields.io/pypi/l/aliceio.svg?style=flat-square">
-  <img alt="Status" src="https://img.shields.io/pypi/status/aliceio.svg?style=flat-square">
-  <img alt="PyPI" src="https://img.shields.io/pypi/v/aliceio?label=pypi&style=flat-square">
-  <img alt="Downloads" src="https://img.shields.io/pypi/dw/aliceio.svg?style=flat-square">
-  <img alt="Supported python versions" src="https://img.shields.io/pypi/pyversions/aliceio.svg?style=flat-square">
-  <img alt="Tests" src="https://img.shields.io/github/actions/workflow/status/K1rL3s/aliceio/tests.yml?style=flat-square">
-</p>
+<div align="center">
+
+[![License](https://img.shields.io/pypi/l/aliceio.svg?style=flat)](https://github.com/K1rL3s/aliceio/blob/master/LICENSE)
+[![Status](https://img.shields.io/pypi/status/aliceio.svg?style=flat)](https://pypi.org/project/aliceio/)
+[![PyPI](https://img.shields.io/pypi/v/aliceio?label=pypi&style=flat)](https://pypi.org/project/aliceio/)
+[![Downloads](https://img.shields.io/pypi/dm/aliceio.svg?style=flat)](https://pypi.org/project/aliceio/)
+[![GitHub Repo stars](https://img.shields.io/github/stars/K1rL3s/aliceio?style=flat)](https://github.com/K1rL3s/aliceio/stargazers)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/aliceio.svg?style=flat)](https://pypi.org/project/aliceio/)
+[![Tests](https://img.shields.io/github/actions/workflow/status/K1rL3s/aliceio/tests.yml?style=flat)](https://github.com/K1rL3s/aliceio/actions)
+[![Coverage](https://codecov.io/gh/K1rL3s/aliceio/graph/badge.svg?style=flat)](https://codecov.io/gh/K1rL3s/aliceio)
+
+</div>
 <p align="center">
     <b>
-        Асинхронный фреймворк для
+        Асинхронный фреймворк, упрощающий разработку
         <a target="_blank" href="https://dialogs.yandex.ru/store">навыков Алисы</a>
         из
         <a target="_blank" href="https://dialogs.yandex.ru/development">Яндекс.Диалогов</a>
     </b>
 </p>
 <p align="center">
     Based on <a target="_blank" href="https://github.com/aiogram/aiogram/tree/dev-3.x">aiogram v3</a>
@@ -123,15 +127,15 @@
 - Машина состояний (Finite State Machine)
 - Мидлвари (для входящих событий и вызовов API)
 - Мощные [магические фильтры](https://github.com/aiogram/magic-filter)
 - Реакция на [долгое время работы](https://yandex.ru/dev/dialogs/alice/doc/publish-settings.html#troubleshooting)
 
 
 ### Важно!
-Настоятельно рекомендуется иметь опыт работы с [asyncio](https://docs.python.org/3/library/asyncio.html) перед использование **aliceio**
+Настоятельно рекомендуется иметь опыт работы с [asyncio](https://docs.python.org/3/library/asyncio.html) перед использованием **aliceio**
 
 
 ## Быстрый старт
 
 Как получить `skill_id` и подключить навык к Алисе можно прочитать <a target="_blank" href="https://aliceio.readthedocs.io/ru/latest/tutorial/start/">тут</a>.
 
 ```python
@@ -167,13 +171,13 @@
 - [Туториал](https://aliceio.readthedocs.io/ru/latest/tutorial/start/)
 - [Документация](https://aliceio.readthedocs.io/)
 - [Примеры](https://github.com/K1rL3s/aliceio/tree/master/examples)
 
 
 ## Связь
 Если у вас есть вопросы, вы можете посетить чат сообщества в Telegram
--   🇷🇺 [\@aliceio_ru](https://t.me/aliceio_ru)
+-   🇷🇺 [\@aliceio_chat](https://t.me/aliceio_chat)
 
 
 ## Лицензия
 Copyright © 2023-2024 [K1rL3s](https://github.com/K1rL3s) and [ZloyKobra](https://github.com/ZloyKobra) \
 Этот проект использует [MIT](https://github.com/K1rL3s/aliceio/blob/master/LICENSE) лицензию
```

