# Comparing `tmp/cfbd-4.4.8.tar.gz` & `tmp/cfbd-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfbd-4.4.8.tar", last modified: Sat Sep 24 17:53:11 2022, max compression
+gzip compressed data, was "cfbd-4.4.9.tar", last modified: Wed Sep 28 22:12:05 2022, max compression
```

## Comparing `cfbd-4.4.8.tar` & `cfbd-4.4.9.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:11.095841 cfbd-4.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-24 17:53:11.095841 cfbd-4.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14444 2022-09-24 17:53:04.000000 cfbd-4.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:11.075841 cfbd-4.4.8/cfbd/
--rw-r--r--   0 runner    (1001) docker     (121)     7775 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:11.075841 cfbd-4.4.8/cfbd/api/
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6225 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/betting_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/coaches_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/conferences_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/draft_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/drives_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    44806 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/games_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    35816 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/metrics_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    23993 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/players_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    23383 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/plays_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5657 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/rankings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    16894 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/ratings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    14471 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/recruiting_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20076 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/stats_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    19593 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3985 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api/venues_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    25243 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:11.087841 cfbd-4.4.8/cfbd/models/
--rw-r--r--   0 runner    (1001) docker     (121)     6990 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_game_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)    17732 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_game_stat_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     6143 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_game_stat_offense_rushing_plays.py
--rw-r--r--   0 runner    (1001) docker     (121)     5386 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_game_stat_offense_standard_downs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_season_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)    20196 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_season_stat_defense.py
--rw-r--r--   0 runner    (1001) docker     (121)    21436 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_season_stat_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     4991 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_season_stat_offense_field_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     6868 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_season_stat_offense_rushing_plays.py
--rw-r--r--   0 runner    (1001) docker     (121)     6107 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/advanced_season_stat_offense_standard_downs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score.py
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_players.py
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_players_average.py
--rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_players_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     9662 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_players_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     9331 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_explosiveness.py
--rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_field_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_havoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6365 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_overall.py
--rw-r--r--   0 runner    (1001) docker     (121)     6254 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)    10512 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_rushing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6243 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_scoring_opportunities.py
--rw-r--r--   0 runner    (1001) docker     (121)     6082 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/box_score_teams_success_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/coach.py
--rw-r--r--   0 runner    (1001) docker     (121)    11296 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/coach_seasons.py
--rw-r--r--   0 runner    (1001) docker     (121)     6185 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/conference.py
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/conference_sp_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     8890 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/conference_sp_rating_defense.py
--rw-r--r--   0 runner    (1001) docker     (121)     9547 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/conference_sp_rating_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)    15563 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/draft_pick.py
--rw-r--r--   0 runner    (1001) docker     (121)     7064 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/draft_pick_hometown_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/draft_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/draft_team.py
--rw-r--r--   0 runner    (1001) docker     (121)    19983 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/drive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4210 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/drive_start_time.py
--rw-r--r--   0 runner    (1001) docker     (121)    25253 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game.py
--rw-r--r--   0 runner    (1001) docker     (121)    10878 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game_lines_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)    10988 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game_media.py
--rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game_ppa_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)    18308 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/game_weather.py
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (121)     9403 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/live_play_by_play.py
--rw-r--r--   0 runner    (1001) docker     (121)    14689 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/live_play_by_play_drives.py
--rw-r--r--   0 runner    (1001) docker     (121)    16653 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/live_play_by_play_plays.py
--rw-r--r--   0 runner    (1001) docker     (121)    22352 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/live_play_by_play_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)    20467 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/play.py
--rw-r--r--   0 runner    (1001) docker     (121)    15032 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/play_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/play_stat_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/play_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    13723 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/play_wp.py
--rw-r--r--   0 runner    (1001) docker     (121)    13278 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player.py
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_athletes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     7381 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_ppa_average_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_school.py
--rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     4246 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_game_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    11047 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_search_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     8207 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_season_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     8809 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_season_ppa_average_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_season_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     7175 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/player_usage_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/portal_player.py
--rw-r--r--   0 runner    (1001) docker     (121)     8450 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/position_group_recruiting_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/predicted_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/pregame_wp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5453 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/ranking_week.py
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/ranking_week_polls.py
--rw-r--r--   0 runner    (1001) docker     (121)     6353 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/ranking_week_ranks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13569 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/recruit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/recruit_hometown_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    14835 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/returning_production.py
--rw-r--r--   0 runner    (1001) docker     (121)    13832 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/scoreboard_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     5976 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/scoreboard_game_betting.py
--rw-r--r--   0 runner    (1001) docker     (121)     6365 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/scoreboard_game_home_team.py
--rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/scoreboard_game_venue.py
--rw-r--r--   0 runner    (1001) docker     (121)     6023 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/scoreboard_game_weather.py
--rw-r--r--   0 runner    (1001) docker     (121)    12330 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_elo_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_game_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_game_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)    11964 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     8042 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_matchup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10310 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_matchup_games.py
--rw-r--r--   0 runner    (1001) docker     (121)     6016 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     7791 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_ppa_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_ppa_offense_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (121)     9047 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     5341 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_record_total.py
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_recruiting_rank.py
--rw-r--r--   0 runner    (1001) docker     (121)    11190 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_season.py
--rw-r--r--   0 runner    (1001) docker     (121)     6223 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_season_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     9620 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_sp_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_sp_rating_defense.py
--rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_sp_rating_defense_havoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9972 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_sp_rating_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_sp_rating_special_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_srs_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/team_talent.py
--rw-r--r--   0 runner    (1001) docker     (121)    10774 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/venue.py
--rw-r--r--   0 runner    (1001) docker     (121)     3969 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/venue_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/models/week.py
--rw-r--r--   0 runner    (1001) docker     (121)    13382 2022-09-24 17:53:04.000000 cfbd-4.4.8/cfbd/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:11.075841 cfbd-4.4.8/cfbd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-24 17:53:11.000000 cfbd-4.4.8/cfbd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-09-24 17:53:11.000000 cfbd-4.4.8/cfbd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-24 17:53:11.000000 cfbd-4.4.8/cfbd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-24 17:53:11.000000 cfbd-4.4.8/cfbd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-24 17:53:11.000000 cfbd-4.4.8/cfbd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-24 17:53:11.095841 cfbd-4.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-09-24 17:53:04.000000 cfbd-4.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:11.095841 cfbd-4.4.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_game_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_game_stat_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_game_stat_offense_rushing_plays.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_game_stat_offense_standard_downs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_season_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_season_stat_defense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_season_stat_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_season_stat_offense_field_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_season_stat_offense_rushing_plays.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_advanced_season_stat_offense_standard_downs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_betting_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_players.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_players_average.py
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_players_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_players_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_explosiveness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_field_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_havoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_overall.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_rushing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_scoring_opportunities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_box_score_teams_success_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_coach.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_coach_seasons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_coaches_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_conference.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_conference_sp_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_conference_sp_rating_defense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_conference_sp_rating_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_conferences_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_draft_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_draft_pick.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_draft_pick_hometown_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_draft_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_draft_team.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_drive_start_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_drives_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game_lines_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game_media.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game_ppa_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_game_weather.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_games_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_live_play_by_play.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_live_play_by_play_drives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_live_play_by_play_plays.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_live_play_by_play_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_metrics_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_play.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_play_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_play_stat_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_play_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_play_wp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_athletes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_ppa_average_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_school.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_game_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_search_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_season_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_season_ppa_average_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_season_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_player_usage_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_players_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_plays_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_portal_player.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_position_group_recruiting_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_predicted_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_pregame_wp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_ranking_week.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_ranking_week_polls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_ranking_week_ranks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_rankings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_ratings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_recruit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_recruit_hometown_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_recruiting_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_returning_production.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_scoreboard_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_scoreboard_game_betting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_scoreboard_game_home_team.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_scoreboard_game_venue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_scoreboard_game_weather.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_stats_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_elo_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_game.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_game_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_game_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_matchup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_matchup_games.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_ppa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_ppa_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_ppa_offense_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_record_total.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_recruiting_rank.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_season.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_season_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_sp_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_sp_rating_defense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_sp_rating_defense_havoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_sp_rating_offense.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_sp_rating_special_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_srs_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_team_talent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_venue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_venue_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_venues_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-24 17:53:04.000000 cfbd-4.4.8/test/test_week.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 22:12:05.176787 cfbd-4.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-28 22:12:05.176787 cfbd-4.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14444 2022-09-28 22:11:56.000000 cfbd-4.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 22:12:05.148785 cfbd-4.4.9/cfbd/
+-rw-r--r--   0 runner    (1001) docker     (121)     7775 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 22:12:05.148785 cfbd-4.4.9/cfbd/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6225 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/betting_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/coaches_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/conferences_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/draft_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/drives_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44806 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/games_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35816 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/metrics_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23993 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/players_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23383 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/plays_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5657 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/rankings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16894 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/ratings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14471 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/recruiting_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20076 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/stats_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19593 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3985 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api/venues_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25243 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 22:12:05.160786 cfbd-4.4.9/cfbd/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     6990 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_game_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17732 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_game_stat_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6143 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_game_stat_offense_rushing_plays.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5386 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_game_stat_offense_standard_downs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_season_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20196 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_season_stat_defense.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21436 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_season_stat_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4991 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_season_stat_offense_field_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6868 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_season_stat_offense_rushing_plays.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6107 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/advanced_season_stat_offense_standard_downs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_players.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_players_average.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_players_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9662 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_players_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9331 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_explosiveness.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_field_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_havoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6365 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_overall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6254 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10512 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_rushing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6243 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_scoring_opportunities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6082 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/box_score_teams_success_rates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/coach.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11296 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/coach_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6185 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/conference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/conference_sp_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8890 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/conference_sp_rating_defense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9547 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/conference_sp_rating_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15563 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/draft_pick.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7064 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/draft_pick_hometown_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/draft_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/draft_team.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19983 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/drive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4210 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/drive_start_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25253 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10878 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game_lines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game_lines_lines.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10988 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game_media.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game_ppa_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18308 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/game_weather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9403 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/live_play_by_play.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14689 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/live_play_by_play_drives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16653 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/live_play_by_play_plays.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22352 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/live_play_by_play_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20467 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/play.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15032 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/play_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/play_stat_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/play_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13723 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/play_wp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13278 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_athletes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7381 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_ppa_average_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_school.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4246 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_game_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11047 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8207 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_season_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8809 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_season_ppa_average_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_season_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7175 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/player_usage_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/portal_player.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8450 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/position_group_recruiting_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/predicted_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/pregame_wp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5453 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/ranking_week.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/ranking_week_polls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6353 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/ranking_week_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13569 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/recruit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/recruit_hometown_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14835 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/returning_production.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13832 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/scoreboard_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5976 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/scoreboard_game_betting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6365 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/scoreboard_game_home_team.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/scoreboard_game_venue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6023 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/scoreboard_game_weather.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12330 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_elo_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_game_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_game_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11964 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8042 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_matchup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10310 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_matchup_games.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6016 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7791 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_ppa_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_ppa_offense_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9047 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5341 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_record_total.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_recruiting_rank.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11190 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_season.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6223 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_season_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9620 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_sp_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_sp_rating_defense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_sp_rating_defense_havoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9972 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_sp_rating_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_sp_rating_special_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_srs_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/team_talent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10774 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/venue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3969 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/venue_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/models/week.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13382 2022-09-28 22:11:56.000000 cfbd-4.4.9/cfbd/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 22:12:05.148785 cfbd-4.4.9/cfbd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-28 22:12:05.000000 cfbd-4.4.9/cfbd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-09-28 22:12:05.000000 cfbd-4.4.9/cfbd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 22:12:05.000000 cfbd-4.4.9/cfbd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-28 22:12:05.000000 cfbd-4.4.9/cfbd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-28 22:12:05.000000 cfbd-4.4.9/cfbd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 22:12:05.176787 cfbd-4.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-09-28 22:11:56.000000 cfbd-4.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 22:12:05.176787 cfbd-4.4.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_game_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_game_stat_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_game_stat_offense_rushing_plays.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_game_stat_offense_standard_downs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_season_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_season_stat_defense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_season_stat_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_season_stat_offense_field_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_season_stat_offense_rushing_plays.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_advanced_season_stat_offense_standard_downs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_betting_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_players.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_players_average.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_players_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_players_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_explosiveness.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_field_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_havoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_overall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_rushing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_scoring_opportunities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_box_score_teams_success_rates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_coach.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_coach_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_coaches_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_conference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_conference_sp_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_conference_sp_rating_defense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_conference_sp_rating_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_conferences_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_draft_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_draft_pick.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_draft_pick_hometown_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_draft_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_draft_team.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_drive_start_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_drives_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game_lines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game_lines_lines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game_media.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game_ppa_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_game_weather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_games_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_live_play_by_play.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_live_play_by_play_drives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_live_play_by_play_plays.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_live_play_by_play_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_metrics_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_play.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_play_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_play_stat_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_play_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_play_wp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_athletes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_ppa_average_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_school.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_game_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_season_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_season_ppa_average_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_season_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_player_usage_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_players_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_plays_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_portal_player.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_position_group_recruiting_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_predicted_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_pregame_wp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_ranking_week.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_ranking_week_polls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_ranking_week_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_rankings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_ratings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_recruit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_recruit_hometown_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_recruiting_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_returning_production.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_scoreboard_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_scoreboard_game_betting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_scoreboard_game_home_team.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_scoreboard_game_venue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_scoreboard_game_weather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_stats_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_elo_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_game_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_game_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_matchup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_matchup_games.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_ppa_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_ppa_offense_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_record_total.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_recruiting_rank.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_season.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_season_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_sp_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_sp_rating_defense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_sp_rating_defense_havoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_sp_rating_offense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_sp_rating_special_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_srs_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_team_talent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_venue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_venue_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_venues_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-28 22:11:56.000000 cfbd-4.4.9/test/test_week.py
```

### Comparing `cfbd-4.4.8/README.md` & `cfbd-4.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cfbd
 This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 4.4.8
-- Package version: 4.4.8
+- API version: 4.4.9
+- Package version: 4.4.9
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `cfbd-4.4.8/cfbd/__init__.py` & `cfbd-4.4.9/cfbd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/__init__.py` & `cfbd-4.4.9/cfbd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cfbd-4.4.8/cfbd/api/betting_api.py` & `cfbd-4.4.9/cfbd/api/betting_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/coaches_api.py` & `cfbd-4.4.9/cfbd/api/coaches_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/conferences_api.py` & `cfbd-4.4.9/cfbd/api/conferences_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/draft_api.py` & `cfbd-4.4.9/cfbd/api/draft_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/drives_api.py` & `cfbd-4.4.9/cfbd/api/drives_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/games_api.py` & `cfbd-4.4.9/cfbd/api/games_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/metrics_api.py` & `cfbd-4.4.9/cfbd/api/metrics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/players_api.py` & `cfbd-4.4.9/cfbd/api/players_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/plays_api.py` & `cfbd-4.4.9/cfbd/api/plays_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/rankings_api.py` & `cfbd-4.4.9/cfbd/api/rankings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/ratings_api.py` & `cfbd-4.4.9/cfbd/api/ratings_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/recruiting_api.py` & `cfbd-4.4.9/cfbd/api/recruiting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/stats_api.py` & `cfbd-4.4.9/cfbd/api/stats_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/teams_api.py` & `cfbd-4.4.9/cfbd/api/teams_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api/venues_api.py` & `cfbd-4.4.9/cfbd/api/venues_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/api_client.py` & `cfbd-4.4.9/cfbd/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import datetime
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/4.4.8/python'
+        self.user_agent = 'Swagger-Codegen/4.4.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `cfbd-4.4.8/cfbd/configuration.py` & `cfbd-4.4.9/cfbd/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -246,10 +246,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.4.8\n"\
-               "SDK Package Version: 4.4.8".\
+               "Version of the API: 4.4.9\n"\
+               "SDK Package Version: 4.4.9".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `cfbd-4.4.8/cfbd/models/__init__.py` & `cfbd-4.4.9/cfbd/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_game_stat.py` & `cfbd-4.4.9/cfbd/models/advanced_game_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_game_stat_offense.py` & `cfbd-4.4.9/cfbd/models/advanced_game_stat_offense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_game_stat_offense_rushing_plays.py` & `cfbd-4.4.9/cfbd/models/advanced_game_stat_offense_rushing_plays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_game_stat_offense_standard_downs.py` & `cfbd-4.4.9/cfbd/models/advanced_game_stat_offense_standard_downs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_season_stat.py` & `cfbd-4.4.9/cfbd/models/advanced_season_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_season_stat_defense.py` & `cfbd-4.4.9/cfbd/models/advanced_season_stat_defense.py`

 * *Files identical despite different names*

### Comparing `cfbd-4.4.8/cfbd/models/advanced_season_stat_offense.py` & `cfbd-4.4.9/cfbd/models/advanced_season_stat_offense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_season_stat_offense_field_position.py` & `cfbd-4.4.9/cfbd/models/advanced_season_stat_offense_field_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_season_stat_offense_rushing_plays.py` & `cfbd-4.4.9/cfbd/models/advanced_season_stat_offense_rushing_plays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/advanced_season_stat_offense_standard_downs.py` & `cfbd-4.4.9/cfbd/models/advanced_season_stat_offense_standard_downs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score.py` & `cfbd-4.4.9/cfbd/models/box_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_players.py` & `cfbd-4.4.9/cfbd/models/box_score_players.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_players_average.py` & `cfbd-4.4.9/cfbd/models/box_score_players_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_players_ppa.py` & `cfbd-4.4.9/cfbd/models/box_score_players_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_players_usage.py` & `cfbd-4.4.9/cfbd/models/box_score_players_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams.py` & `cfbd-4.4.9/cfbd/models/box_score_teams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_explosiveness.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_explosiveness.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_field_position.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_field_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_havoc.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_havoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_overall.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_overall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_ppa.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_rushing.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_rushing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_scoring_opportunities.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_scoring_opportunities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/box_score_teams_success_rates.py` & `cfbd-4.4.9/cfbd/models/box_score_teams_success_rates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/coach.py` & `cfbd-4.4.9/cfbd/models/coach.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/coach_seasons.py` & `cfbd-4.4.9/cfbd/models/coach_seasons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/conference.py` & `cfbd-4.4.9/cfbd/models/conference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/conference_sp_rating.py` & `cfbd-4.4.9/cfbd/models/conference_sp_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/conference_sp_rating_defense.py` & `cfbd-4.4.9/cfbd/models/conference_sp_rating_defense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/conference_sp_rating_offense.py` & `cfbd-4.4.9/cfbd/models/conference_sp_rating_offense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/draft_pick.py` & `cfbd-4.4.9/cfbd/models/draft_pick.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/draft_pick_hometown_info.py` & `cfbd-4.4.9/cfbd/models/draft_pick_hometown_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/draft_position.py` & `cfbd-4.4.9/cfbd/models/draft_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/draft_team.py` & `cfbd-4.4.9/cfbd/models/draft_team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/drive.py` & `cfbd-4.4.9/cfbd/models/drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/drive_start_time.py` & `cfbd-4.4.9/cfbd/models/drive_start_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game.py` & `cfbd-4.4.9/cfbd/models/game.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game_lines.py` & `cfbd-4.4.9/cfbd/models/game_lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game_lines_lines.py` & `cfbd-4.4.9/cfbd/models/game_lines_lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game_media.py` & `cfbd-4.4.9/cfbd/models/game_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game_ppa.py` & `cfbd-4.4.9/cfbd/models/game_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game_ppa_offense.py` & `cfbd-4.4.9/cfbd/models/game_ppa_offense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/game_weather.py` & `cfbd-4.4.9/cfbd/models/game_weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/inline_response200.py` & `cfbd-4.4.9/cfbd/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `cfbd-4.4.8/cfbd/models/live_play_by_play.py` & `cfbd-4.4.9/cfbd/models/live_play_by_play.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/live_play_by_play_drives.py` & `cfbd-4.4.9/cfbd/models/live_play_by_play_drives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/live_play_by_play_plays.py` & `cfbd-4.4.9/cfbd/models/live_play_by_play_plays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/live_play_by_play_teams.py` & `cfbd-4.4.9/cfbd/models/live_play_by_play_teams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/play.py` & `cfbd-4.4.9/cfbd/models/play.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/play_stat.py` & `cfbd-4.4.9/cfbd/models/play_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/play_stat_type.py` & `cfbd-4.4.9/cfbd/models/play_stat_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/play_type.py` & `cfbd-4.4.9/cfbd/models/play_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/play_wp.py` & `cfbd-4.4.9/cfbd/models/play_wp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player.py` & `cfbd-4.4.9/cfbd/models/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game.py` & `cfbd-4.4.9/cfbd/models/player_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_athletes.py` & `cfbd-4.4.9/cfbd/models/player_game_athletes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_categories.py` & `cfbd-4.4.9/cfbd/models/player_game_categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_ppa.py` & `cfbd-4.4.9/cfbd/models/player_game_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_ppa_average_ppa.py` & `cfbd-4.4.9/cfbd/models/player_game_ppa_average_ppa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_school.py` & `cfbd-4.4.9/cfbd/models/player_game_school.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_teams.py` & `cfbd-4.4.9/cfbd/models/player_game_teams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_game_types.py` & `cfbd-4.4.9/cfbd/models/player_game_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_search_result.py` & `cfbd-4.4.9/cfbd/models/player_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_season_ppa.py` & `cfbd-4.4.9/cfbd/models/player_season_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_season_ppa_average_ppa.py` & `cfbd-4.4.9/cfbd/models/player_season_ppa_average_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_season_stat.py` & `cfbd-4.4.9/cfbd/models/player_season_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_usage.py` & `cfbd-4.4.9/cfbd/models/player_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/player_usage_usage.py` & `cfbd-4.4.9/cfbd/models/player_usage_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/portal_player.py` & `cfbd-4.4.9/cfbd/models/portal_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/position_group_recruiting_rating.py` & `cfbd-4.4.9/cfbd/models/position_group_recruiting_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/predicted_points.py` & `cfbd-4.4.9/cfbd/models/predicted_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/pregame_wp.py` & `cfbd-4.4.9/cfbd/models/pregame_wp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/ranking_week.py` & `cfbd-4.4.9/cfbd/models/ranking_week.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/ranking_week_polls.py` & `cfbd-4.4.9/cfbd/models/ranking_week_polls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/ranking_week_ranks.py` & `cfbd-4.4.9/cfbd/models/ranking_week_ranks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/recruit.py` & `cfbd-4.4.9/cfbd/models/recruit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/recruit_hometown_info.py` & `cfbd-4.4.9/cfbd/models/recruit_hometown_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/returning_production.py` & `cfbd-4.4.9/cfbd/models/returning_production.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/scoreboard_game.py` & `cfbd-4.4.9/cfbd/models/scoreboard_game.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/scoreboard_game_betting.py` & `cfbd-4.4.9/cfbd/models/scoreboard_game_betting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/scoreboard_game_home_team.py` & `cfbd-4.4.9/cfbd/models/scoreboard_game_home_team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/scoreboard_game_venue.py` & `cfbd-4.4.9/cfbd/models/scoreboard_game_venue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/scoreboard_game_weather.py` & `cfbd-4.4.9/cfbd/models/scoreboard_game_weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team.py` & `cfbd-4.4.9/cfbd/models/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_elo_rating.py` & `cfbd-4.4.9/cfbd/models/team_elo_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_game.py` & `cfbd-4.4.9/cfbd/models/team_game.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_game_stats.py` & `cfbd-4.4.9/cfbd/models/team_game_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_game_teams.py` & `cfbd-4.4.9/cfbd/models/team_game_teams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -31,15 +31,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'school': 'str',
         'conference': 'str',
-        'home_away': 'bool',
+        'home_away': 'str',
         'points': 'int',
         'stats': 'list[TeamGameStats]'
     }
 
     attribute_map = {
         'school': 'school',
         'conference': 'conference',
@@ -116,25 +116,25 @@
 
     @property
     def home_away(self):
         """Gets the home_away of this TeamGameTeams.  # noqa: E501
 
 
         :return: The home_away of this TeamGameTeams.  # noqa: E501
-        :rtype: bool
+        :rtype: str
         """
         return self._home_away
 
     @home_away.setter
     def home_away(self, home_away):
         """Sets the home_away of this TeamGameTeams.
 
 
         :param home_away: The home_away of this TeamGameTeams.  # noqa: E501
-        :type: bool
+        :type: str
         """
 
         self._home_away = home_away
 
     @property
     def points(self):
         """Gets the points of this TeamGameTeams.  # noqa: E501
```

### Comparing `cfbd-4.4.8/cfbd/models/team_location.py` & `cfbd-4.4.9/cfbd/models/team_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_matchup.py` & `cfbd-4.4.9/cfbd/models/team_matchup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_matchup_games.py` & `cfbd-4.4.9/cfbd/models/team_matchup_games.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_ppa.py` & `cfbd-4.4.9/cfbd/models/team_ppa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_ppa_offense.py` & `cfbd-4.4.9/cfbd/models/team_ppa_offense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_ppa_offense_cumulative.py` & `cfbd-4.4.9/cfbd/models/team_ppa_offense_cumulative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_record.py` & `cfbd-4.4.9/cfbd/models/team_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_record_total.py` & `cfbd-4.4.9/cfbd/models/team_record_total.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_recruiting_rank.py` & `cfbd-4.4.9/cfbd/models/team_recruiting_rank.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_season.py` & `cfbd-4.4.9/cfbd/models/team_season.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_season_stat.py` & `cfbd-4.4.9/cfbd/models/team_season_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_sp_rating.py` & `cfbd-4.4.9/cfbd/models/team_sp_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_sp_rating_defense.py` & `cfbd-4.4.9/cfbd/models/team_sp_rating_defense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_sp_rating_defense_havoc.py` & `cfbd-4.4.9/cfbd/models/team_sp_rating_defense_havoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_sp_rating_offense.py` & `cfbd-4.4.9/cfbd/models/team_sp_rating_offense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_sp_rating_special_teams.py` & `cfbd-4.4.9/cfbd/models/team_sp_rating_special_teams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_srs_rating.py` & `cfbd-4.4.9/cfbd/models/team_srs_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/team_talent.py` & `cfbd-4.4.9/cfbd/models/team_talent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/venue.py` & `cfbd-4.4.9/cfbd/models/venue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/venue_location.py` & `cfbd-4.4.9/cfbd/models/venue_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/models/week.py` & `cfbd-4.4.9/cfbd/models/week.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `cfbd-4.4.8/cfbd/rest.py` & `cfbd-4.4.9/cfbd/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/cfbd.egg-info/SOURCES.txt` & `cfbd-4.4.9/cfbd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfbd-4.4.8/setup.py` & `cfbd-4.4.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "cfbd"
-VERSION = "4.4.8"
+VERSION = "4.4.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `cfbd-4.4.8/test/test_advanced_game_stat.py` & `cfbd-4.4.9/test/test_advanced_game_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_game_stat_offense.py` & `cfbd-4.4.9/test/test_advanced_game_stat_offense.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_game_stat_offense_rushing_plays.py` & `cfbd-4.4.9/test/test_advanced_game_stat_offense_rushing_plays.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_game_stat_offense_standard_downs.py` & `cfbd-4.4.9/test/test_advanced_game_stat_offense_standard_downs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_season_stat.py` & `cfbd-4.4.9/test/test_advanced_season_stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_season_stat_defense.py` & `cfbd-4.4.9/test/test_advanced_season_stat_defense.py`

 * *Files identical despite different names*

### Comparing `cfbd-4.4.8/test/test_advanced_season_stat_offense.py` & `cfbd-4.4.9/test/test_advanced_season_stat_offense.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_season_stat_offense_field_position.py` & `cfbd-4.4.9/test/test_advanced_season_stat_offense_field_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_season_stat_offense_rushing_plays.py` & `cfbd-4.4.9/test/test_advanced_season_stat_offense_rushing_plays.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_advanced_season_stat_offense_standard_downs.py` & `cfbd-4.4.9/test/test_advanced_season_stat_offense_standard_downs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_betting_api.py` & `cfbd-4.4.9/test/test_betting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score.py` & `cfbd-4.4.9/test/test_box_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_players.py` & `cfbd-4.4.9/test/test_box_score_players.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_players_average.py` & `cfbd-4.4.9/test/test_box_score_players_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_players_ppa.py` & `cfbd-4.4.9/test/test_box_score_players_ppa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_players_usage.py` & `cfbd-4.4.9/test/test_box_score_players_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams.py` & `cfbd-4.4.9/test/test_box_score_teams_overall.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.box_score_teams import BoxScoreTeams  # noqa: E501
+from cfbd.models.box_score_teams_overall import BoxScoreTeamsOverall  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestBoxScoreTeams(unittest.TestCase):
-    """BoxScoreTeams unit test stubs"""
+class TestBoxScoreTeamsOverall(unittest.TestCase):
+    """BoxScoreTeamsOverall unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBoxScoreTeams(self):
-        """Test BoxScoreTeams"""
+    def testBoxScoreTeamsOverall(self):
+        """Test BoxScoreTeamsOverall"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.box_score_teams.BoxScoreTeams()  # noqa: E501
+        # model = cfbd.models.box_score_teams_overall.BoxScoreTeamsOverall()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_explosiveness.py` & `cfbd-4.4.9/test/test_box_score_teams_explosiveness.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_field_position.py` & `cfbd-4.4.9/test/test_box_score_teams_field_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_havoc.py` & `cfbd-4.4.9/test/test_box_score_teams_havoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_overall.py` & `cfbd-4.4.9/test/test_box_score_teams_ppa.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.box_score_teams_overall import BoxScoreTeamsOverall  # noqa: E501
+from cfbd.models.box_score_teams_ppa import BoxScoreTeamsPpa  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestBoxScoreTeamsOverall(unittest.TestCase):
-    """BoxScoreTeamsOverall unit test stubs"""
+class TestBoxScoreTeamsPpa(unittest.TestCase):
+    """BoxScoreTeamsPpa unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBoxScoreTeamsOverall(self):
-        """Test BoxScoreTeamsOverall"""
+    def testBoxScoreTeamsPpa(self):
+        """Test BoxScoreTeamsPpa"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.box_score_teams_overall.BoxScoreTeamsOverall()  # noqa: E501
+        # model = cfbd.models.box_score_teams_ppa.BoxScoreTeamsPpa()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_ppa.py` & `cfbd-4.4.9/test/test_box_score_teams_rushing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.box_score_teams_ppa import BoxScoreTeamsPpa  # noqa: E501
+from cfbd.models.box_score_teams_rushing import BoxScoreTeamsRushing  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestBoxScoreTeamsPpa(unittest.TestCase):
-    """BoxScoreTeamsPpa unit test stubs"""
+class TestBoxScoreTeamsRushing(unittest.TestCase):
+    """BoxScoreTeamsRushing unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBoxScoreTeamsPpa(self):
-        """Test BoxScoreTeamsPpa"""
+    def testBoxScoreTeamsRushing(self):
+        """Test BoxScoreTeamsRushing"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.box_score_teams_ppa.BoxScoreTeamsPpa()  # noqa: E501
+        # model = cfbd.models.box_score_teams_rushing.BoxScoreTeamsRushing()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_rushing.py` & `cfbd-4.4.9/test/test_box_score_teams.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.box_score_teams_rushing import BoxScoreTeamsRushing  # noqa: E501
+from cfbd.models.box_score_teams import BoxScoreTeams  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestBoxScoreTeamsRushing(unittest.TestCase):
-    """BoxScoreTeamsRushing unit test stubs"""
+class TestBoxScoreTeams(unittest.TestCase):
+    """BoxScoreTeams unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBoxScoreTeamsRushing(self):
-        """Test BoxScoreTeamsRushing"""
+    def testBoxScoreTeams(self):
+        """Test BoxScoreTeams"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.box_score_teams_rushing.BoxScoreTeamsRushing()  # noqa: E501
+        # model = cfbd.models.box_score_teams.BoxScoreTeams()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_scoring_opportunities.py` & `cfbd-4.4.9/test/test_box_score_teams_scoring_opportunities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_box_score_teams_success_rates.py` & `cfbd-4.4.9/test/test_box_score_teams_success_rates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_coach.py` & `cfbd-4.4.9/test/test_coach.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_coach_seasons.py` & `cfbd-4.4.9/test/test_coach_seasons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_coaches_api.py` & `cfbd-4.4.9/test/test_coaches_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_conference.py` & `cfbd-4.4.9/test/test_team_game.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.conference import Conference  # noqa: E501
+from cfbd.models.team_game import TeamGame  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestConference(unittest.TestCase):
-    """Conference unit test stubs"""
+class TestTeamGame(unittest.TestCase):
+    """TeamGame unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testConference(self):
-        """Test Conference"""
+    def testTeamGame(self):
+        """Test TeamGame"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.conference.Conference()  # noqa: E501
+        # model = cfbd.models.team_game.TeamGame()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_conference_sp_rating.py` & `cfbd-4.4.9/test/test_conference_sp_rating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_conference_sp_rating_defense.py` & `cfbd-4.4.9/test/test_conference_sp_rating_defense.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_conference_sp_rating_offense.py` & `cfbd-4.4.9/test/test_conference_sp_rating_offense.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_conferences_api.py` & `cfbd-4.4.9/test/test_conferences_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_draft_api.py` & `cfbd-4.4.9/test/test_draft_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_draft_pick.py` & `cfbd-4.4.9/test/test_team.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.draft_pick import DraftPick  # noqa: E501
+from cfbd.models.team import Team  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestDraftPick(unittest.TestCase):
-    """DraftPick unit test stubs"""
+class TestTeam(unittest.TestCase):
+    """Team unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDraftPick(self):
-        """Test DraftPick"""
+    def testTeam(self):
+        """Test Team"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.draft_pick.DraftPick()  # noqa: E501
+        # model = cfbd.models.team.Team()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_draft_pick_hometown_info.py` & `cfbd-4.4.9/test/test_draft_pick_hometown_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_draft_position.py` & `cfbd-4.4.9/test/test_draft_position.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_draft_team.py` & `cfbd-4.4.9/test/test_draft_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_drive.py` & `cfbd-4.4.9/test/test_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_drive_start_time.py` & `cfbd-4.4.9/test/test_drive_start_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_drives_api.py` & `cfbd-4.4.9/test/test_drives_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_game.py` & `cfbd-4.4.9/test/test_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_game_lines.py` & `cfbd-4.4.9/test/test_game_lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_game_lines_lines.py` & `cfbd-4.4.9/test/test_game_lines_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_game_media.py` & `cfbd-4.4.9/test/test_game_weather.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.game_media import GameMedia  # noqa: E501
+from cfbd.models.game_weather import GameWeather  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestGameMedia(unittest.TestCase):
-    """GameMedia unit test stubs"""
+class TestGameWeather(unittest.TestCase):
+    """GameWeather unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGameMedia(self):
-        """Test GameMedia"""
+    def testGameWeather(self):
+        """Test GameWeather"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.game_media.GameMedia()  # noqa: E501
+        # model = cfbd.models.game_weather.GameWeather()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_game_ppa.py` & `cfbd-4.4.9/test/test_game_ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_game_ppa_offense.py` & `cfbd-4.4.9/test/test_game_ppa_offense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_game_weather.py` & `cfbd-4.4.9/test/test_scoreboard_game_weather.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.game_weather import GameWeather  # noqa: E501
+from cfbd.models.scoreboard_game_weather import ScoreboardGameWeather  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestGameWeather(unittest.TestCase):
-    """GameWeather unit test stubs"""
+class TestScoreboardGameWeather(unittest.TestCase):
+    """ScoreboardGameWeather unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGameWeather(self):
-        """Test GameWeather"""
+    def testScoreboardGameWeather(self):
+        """Test ScoreboardGameWeather"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.game_weather.GameWeather()  # noqa: E501
+        # model = cfbd.models.scoreboard_game_weather.ScoreboardGameWeather()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_games_api.py` & `cfbd-4.4.9/test/test_games_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_inline_response200.py` & `cfbd-4.4.9/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `cfbd-4.4.8/test/test_live_play_by_play.py` & `cfbd-4.4.9/test/test_live_play_by_play.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_live_play_by_play_drives.py` & `cfbd-4.4.9/test/test_live_play_by_play_drives.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_live_play_by_play_plays.py` & `cfbd-4.4.9/test/test_live_play_by_play_plays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_live_play_by_play_teams.py` & `cfbd-4.4.9/test/test_live_play_by_play_teams.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_metrics_api.py` & `cfbd-4.4.9/test/test_metrics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_play.py` & `cfbd-4.4.9/test/test_play.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_play_stat.py` & `cfbd-4.4.9/test/test_play_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_play_stat_type.py` & `cfbd-4.4.9/test/test_play_stat_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_play_type.py` & `cfbd-4.4.9/test/test_play_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_play_wp.py` & `cfbd-4.4.9/test/test_play_wp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player.py` & `cfbd-4.4.9/test/test_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game.py` & `cfbd-4.4.9/test/test_player_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_athletes.py` & `cfbd-4.4.9/test/test_player_game_athletes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_categories.py` & `cfbd-4.4.9/test/test_player_game_categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_ppa.py` & `cfbd-4.4.9/test/test_player_game_ppa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_ppa_average_ppa.py` & `cfbd-4.4.9/test/test_player_game_ppa_average_ppa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_school.py` & `cfbd-4.4.9/test/test_player_game_school.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_teams.py` & `cfbd-4.4.9/test/test_player_game_teams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_game_types.py` & `cfbd-4.4.9/test/test_player_game_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_search_result.py` & `cfbd-4.4.9/test/test_player_search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_season_ppa.py` & `cfbd-4.4.9/test/test_player_season_ppa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_season_ppa_average_ppa.py` & `cfbd-4.4.9/test/test_player_season_ppa_average_ppa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_season_stat.py` & `cfbd-4.4.9/test/test_player_season_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_usage.py` & `cfbd-4.4.9/test/test_player_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_player_usage_usage.py` & `cfbd-4.4.9/test/test_player_usage_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_players_api.py` & `cfbd-4.4.9/test/test_players_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_plays_api.py` & `cfbd-4.4.9/test/test_plays_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_portal_player.py` & `cfbd-4.4.9/test/test_portal_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_position_group_recruiting_rating.py` & `cfbd-4.4.9/test/test_position_group_recruiting_rating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_predicted_points.py` & `cfbd-4.4.9/test/test_predicted_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_pregame_wp.py` & `cfbd-4.4.9/test/test_pregame_wp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_ranking_week.py` & `cfbd-4.4.9/test/test_ranking_week_ranks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.ranking_week import RankingWeek  # noqa: E501
+from cfbd.models.ranking_week_ranks import RankingWeekRanks  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestRankingWeek(unittest.TestCase):
-    """RankingWeek unit test stubs"""
+class TestRankingWeekRanks(unittest.TestCase):
+    """RankingWeekRanks unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRankingWeek(self):
-        """Test RankingWeek"""
+    def testRankingWeekRanks(self):
+        """Test RankingWeekRanks"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.ranking_week.RankingWeek()  # noqa: E501
+        # model = cfbd.models.ranking_week_ranks.RankingWeekRanks()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_ranking_week_polls.py` & `cfbd-4.4.9/test/test_ranking_week_polls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_ranking_week_ranks.py` & `cfbd-4.4.9/test/test_rankings_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.ranking_week_ranks import RankingWeekRanks  # noqa: E501
+from cfbd.api.rankings_api import RankingsApi  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestRankingWeekRanks(unittest.TestCase):
-    """RankingWeekRanks unit test stubs"""
+class TestRankingsApi(unittest.TestCase):
+    """RankingsApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = cfbd.api.rankings_api.RankingsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testRankingWeekRanks(self):
-        """Test RankingWeekRanks"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.ranking_week_ranks.RankingWeekRanks()  # noqa: E501
+    def test_get_rankings(self):
+        """Test case for get_rankings
+
+        Historical polls and rankings  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_rankings_api.py` & `cfbd-4.4.9/test/test_venue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.api.rankings_api import RankingsApi  # noqa: E501
+from cfbd.models.venue import Venue  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestRankingsApi(unittest.TestCase):
-    """RankingsApi unit test stubs"""
+class TestVenue(unittest.TestCase):
+    """Venue unit test stubs"""
 
     def setUp(self):
-        self.api = cfbd.api.rankings_api.RankingsApi()  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    def test_get_rankings(self):
-        """Test case for get_rankings
-
-        Historical polls and rankings  # noqa: E501
-        """
+    def testVenue(self):
+        """Test Venue"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = cfbd.models.venue.Venue()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_ratings_api.py` & `cfbd-4.4.9/test/test_ratings_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_recruit.py` & `cfbd-4.4.9/test/test_recruit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_recruit_hometown_info.py` & `cfbd-4.4.9/test/test_recruit_hometown_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_recruiting_api.py` & `cfbd-4.4.9/test/test_recruiting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_returning_production.py` & `cfbd-4.4.9/test/test_returning_production.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_scoreboard_game.py` & `cfbd-4.4.9/test/test_scoreboard_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_scoreboard_game_betting.py` & `cfbd-4.4.9/test/test_scoreboard_game_betting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_scoreboard_game_home_team.py` & `cfbd-4.4.9/test/test_scoreboard_game_home_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_scoreboard_game_venue.py` & `cfbd-4.4.9/test/test_scoreboard_game_venue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_scoreboard_game_weather.py` & `cfbd-4.4.9/test/test_team_record_total.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.scoreboard_game_weather import ScoreboardGameWeather  # noqa: E501
+from cfbd.models.team_record_total import TeamRecordTotal  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestScoreboardGameWeather(unittest.TestCase):
-    """ScoreboardGameWeather unit test stubs"""
+class TestTeamRecordTotal(unittest.TestCase):
+    """TeamRecordTotal unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreboardGameWeather(self):
-        """Test ScoreboardGameWeather"""
+    def testTeamRecordTotal(self):
+        """Test TeamRecordTotal"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.scoreboard_game_weather.ScoreboardGameWeather()  # noqa: E501
+        # model = cfbd.models.team_record_total.TeamRecordTotal()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_stats_api.py` & `cfbd-4.4.9/test/test_stats_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team.py` & `cfbd-4.4.9/test/test_week.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.team import Team  # noqa: E501
+from cfbd.models.week import Week  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestTeam(unittest.TestCase):
-    """Team unit test stubs"""
+class TestWeek(unittest.TestCase):
+    """Week unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTeam(self):
-        """Test Team"""
+    def testWeek(self):
+        """Test Week"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.team.Team()  # noqa: E501
+        # model = cfbd.models.week.Week()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_team_elo_rating.py` & `cfbd-4.4.9/test/test_team_elo_rating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_game.py` & `cfbd-4.4.9/test/test_conference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.team_game import TeamGame  # noqa: E501
+from cfbd.models.conference import Conference  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestTeamGame(unittest.TestCase):
-    """TeamGame unit test stubs"""
+class TestConference(unittest.TestCase):
+    """Conference unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTeamGame(self):
-        """Test TeamGame"""
+    def testConference(self):
+        """Test Conference"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.team_game.TeamGame()  # noqa: E501
+        # model = cfbd.models.conference.Conference()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_team_game_stats.py` & `cfbd-4.4.9/test/test_team_game_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_game_teams.py` & `cfbd-4.4.9/test/test_team_game_teams.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_location.py` & `cfbd-4.4.9/test/test_team_location.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_matchup.py` & `cfbd-4.4.9/test/test_team_matchup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_matchup_games.py` & `cfbd-4.4.9/test/test_team_matchup_games.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_ppa.py` & `cfbd-4.4.9/test/test_team_ppa.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_ppa_offense.py` & `cfbd-4.4.9/test/test_team_ppa_offense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_ppa_offense_cumulative.py` & `cfbd-4.4.9/test/test_team_ppa_offense_cumulative.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_record.py` & `cfbd-4.4.9/test/test_team_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_record_total.py` & `cfbd-4.4.9/test/test_team_talent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.team_record_total import TeamRecordTotal  # noqa: E501
+from cfbd.models.team_talent import TeamTalent  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestTeamRecordTotal(unittest.TestCase):
-    """TeamRecordTotal unit test stubs"""
+class TestTeamTalent(unittest.TestCase):
+    """TeamTalent unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTeamRecordTotal(self):
-        """Test TeamRecordTotal"""
+    def testTeamTalent(self):
+        """Test TeamTalent"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.team_record_total.TeamRecordTotal()  # noqa: E501
+        # model = cfbd.models.team_talent.TeamTalent()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_team_recruiting_rank.py` & `cfbd-4.4.9/test/test_team_recruiting_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_season.py` & `cfbd-4.4.9/test/test_team_season.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_season_stat.py` & `cfbd-4.4.9/test/test_team_season_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_sp_rating.py` & `cfbd-4.4.9/test/test_team_sp_rating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_sp_rating_defense.py` & `cfbd-4.4.9/test/test_team_sp_rating_defense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_sp_rating_defense_havoc.py` & `cfbd-4.4.9/test/test_team_sp_rating_defense_havoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_sp_rating_offense.py` & `cfbd-4.4.9/test/test_team_sp_rating_offense.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_sp_rating_special_teams.py` & `cfbd-4.4.9/test/test_team_sp_rating_special_teams.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_srs_rating.py` & `cfbd-4.4.9/test/test_team_srs_rating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_team_talent.py` & `cfbd-4.4.9/test/test_game_media.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.team_talent import TeamTalent  # noqa: E501
+from cfbd.models.game_media import GameMedia  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestTeamTalent(unittest.TestCase):
-    """TeamTalent unit test stubs"""
+class TestGameMedia(unittest.TestCase):
+    """GameMedia unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTeamTalent(self):
-        """Test TeamTalent"""
+    def testGameMedia(self):
+        """Test GameMedia"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.team_talent.TeamTalent()  # noqa: E501
+        # model = cfbd.models.game_media.GameMedia()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_teams_api.py` & `cfbd-4.4.9/test/test_teams_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `cfbd-4.4.8/test/test_venue.py` & `cfbd-4.4.9/test/test_venue_location.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.venue import Venue  # noqa: E501
+from cfbd.models.venue_location import VenueLocation  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestVenue(unittest.TestCase):
-    """Venue unit test stubs"""
+class TestVenueLocation(unittest.TestCase):
+    """VenueLocation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVenue(self):
-        """Test Venue"""
+    def testVenueLocation(self):
+        """Test VenueLocation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.venue.Venue()  # noqa: E501
+        # model = cfbd.models.venue_location.VenueLocation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_venue_location.py` & `cfbd-4.4.9/test/test_venues_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.venue_location import VenueLocation  # noqa: E501
+from cfbd.api.venues_api import VenuesApi  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestVenueLocation(unittest.TestCase):
-    """VenueLocation unit test stubs"""
+class TestVenuesApi(unittest.TestCase):
+    """VenuesApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = cfbd.api.venues_api.VenuesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testVenueLocation(self):
-        """Test VenueLocation"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.venue_location.VenueLocation()  # noqa: E501
+    def test_get_venues(self):
+        """Test case for get_venues
+
+        Arena and venue information  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cfbd-4.4.8/test/test_week.py` & `cfbd-4.4.9/test/test_ranking_week.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     College Football Data API
 
     This is an API for accessing all sorts of college football data.  Please note that API keys should be supplied with \"Bearer \" prepended (e.g. \"Bearer your_key\"). API keys can be acquired from the CollegeFootballData.com website.  # noqa: E501
 
-    OpenAPI spec version: 4.4.8
+    OpenAPI spec version: 4.4.9
     Contact: admin@collegefootballdata.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cfbd
-from cfbd.models.week import Week  # noqa: E501
+from cfbd.models.ranking_week import RankingWeek  # noqa: E501
 from cfbd.rest import ApiException
 
 
-class TestWeek(unittest.TestCase):
-    """Week unit test stubs"""
+class TestRankingWeek(unittest.TestCase):
+    """RankingWeek unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWeek(self):
-        """Test Week"""
+    def testRankingWeek(self):
+        """Test RankingWeek"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cfbd.models.week.Week()  # noqa: E501
+        # model = cfbd.models.ranking_week.RankingWeek()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

