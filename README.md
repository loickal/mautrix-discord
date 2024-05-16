# mautrix-discord

![Version: 0.0.1](https://img.shields.io/badge/Version-0.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.6.5](https://img.shields.io/badge/AppVersion-0.6.5-informational?style=flat-square)

A Matrix-Discord puppeting bridge.

**Homepage:** <https://matrix.to/#/#discord:maunium.net>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Loic Kalbermatter | <loic.kalbermatter@pulseflow.ch> |  |

## Source Code

* <https://github.com/mautrix/discord>
* <https://code.pulseflow.ch/PulseDev/mautrix-discord>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| config.appservice.address | string | `""` |  |
| config.appservice.as_token | string | `"This value is generated when generating the registration"` |  |
| config.appservice.async_transactions | bool | `false` |  |
| config.appservice.bot.avatar | string | `"mxc://maunium.net/nIdEykemnwdisvHbpxflpDlC"` |  |
| config.appservice.bot.displayname | string | `"Discord bridge bot"` |  |
| config.appservice.bot.username | string | `"discordbot"` |  |
| config.appservice.database.max_conn_idle_time | string | `nil` |  |
| config.appservice.database.max_conn_lifetime | string | `nil` |  |
| config.appservice.database.max_idle_conns | int | `2` |  |
| config.appservice.database.max_open_conns | int | `20` |  |
| config.appservice.database.type | string | `"postgres"` |  |
| config.appservice.database.uri | string | `"postgres://user:password@host/database?sslmode=disable"` |  |
| config.appservice.ephemeral_events | bool | `true` |  |
| config.appservice.hostname | string | `"0.0.0.0"` |  |
| config.appservice.hs_token | string | `"This value is generated when generating the registration"` |  |
| config.appservice.id | string | `"discord"` |  |
| config.appservice.port | int | `29334` |  |
| config.bridge.animated_sticker.args.fps | int | `25` |  |
| config.bridge.animated_sticker.args.height | int | `320` |  |
| config.bridge.animated_sticker.args.width | int | `320` |  |
| config.bridge.animated_sticker.target | string | `"webp"` |  |
| config.bridge.autojoin_thread_on_open | bool | `true` |  |
| config.bridge.backfill.forward_limits.initial.channel | int | `0` |  |
| config.bridge.backfill.forward_limits.initial.dm | int | `0` |  |
| config.bridge.backfill.forward_limits.initial.thread | int | `0` |  |
| config.bridge.backfill.forward_limits.missed.channel | int | `0` |  |
| config.bridge.backfill.forward_limits.missed.dm | int | `0` |  |
| config.bridge.backfill.forward_limits.missed.thread | int | `0` |  |
| config.bridge.backfill.max_guild_members | int | `-1` |  |
| config.bridge.cache_media | string | `"unencrypted"` |  |
| config.bridge.channel_name_template | string | `"{{ \"{{if or (eq .Type 3) (eq .Type 4)}}{{.Name}}{{else if eq .Type 1}}{{.Name}} (Discord){{else}}#{{.Name}}{{end}}\" }}"` |  |
| config.bridge.command_prefix | string | `"!discord"` |  |
| config.bridge.custom_emoji_reactions | bool | `true` |  |
| config.bridge.delete_portal_on_channel_delete | bool | `false` |  |
| config.bridge.delivery_receipts | bool | `false` |  |
| config.bridge.displayname_template | string | `"{{ \"{{or .GlobalName .Username}}{{if .Bot}} (bot){{end}} (Discord)\" }}"` |  |
| config.bridge.double_puppet_allow_discovery | bool | `false` |  |
| config.bridge.double_puppet_server_map | object | `{}` |  |
| config.bridge.embed_fields_as_tables | bool | `true` |  |
| config.bridge.enable_webhook_avatars | bool | `true` |  |
| config.bridge.encryption.allow | bool | `false` |  |
| config.bridge.encryption.allow_key_sharing | bool | `false` |  |
| config.bridge.encryption.appservice | bool | `false` |  |
| config.bridge.encryption.default | bool | `false` |  |
| config.bridge.encryption.delete_keys.delete_fully_used_on_decrypt | bool | `false` |  |
| config.bridge.encryption.delete_keys.delete_on_device_delete | bool | `false` |  |
| config.bridge.encryption.delete_keys.delete_outbound_on_ack | bool | `false` |  |
| config.bridge.encryption.delete_keys.delete_outdated_inbound | bool | `false` |  |
| config.bridge.encryption.delete_keys.delete_prev_on_new_session | bool | `false` |  |
| config.bridge.encryption.delete_keys.dont_store_outbound | bool | `false` |  |
| config.bridge.encryption.delete_keys.periodically_delete_expired | bool | `false` |  |
| config.bridge.encryption.delete_keys.ratchet_on_decrypt | bool | `false` |  |
| config.bridge.encryption.plaintext_mentions | bool | `false` |  |
| config.bridge.encryption.require | bool | `false` |  |
| config.bridge.encryption.rotation.disable_device_change_key_rotation | bool | `false` |  |
| config.bridge.encryption.rotation.enable_custom | bool | `false` |  |
| config.bridge.encryption.rotation.messages | int | `100` |  |
| config.bridge.encryption.rotation.milliseconds | int | `604800000` |  |
| config.bridge.encryption.verification_levels.receive | string | `"unverified"` |  |
| config.bridge.encryption.verification_levels.send | string | `"unverified"` |  |
| config.bridge.encryption.verification_levels.share | string | `"cross-signed-tofu"` |  |
| config.bridge.federate_rooms | bool | `true` |  |
| config.bridge.guild_name_template | string | `"{{ \"{{.Name}}\" }}"` |  |
| config.bridge.login_shared_secret_map | object | `{}` |  |
| config.bridge.management_room_text.additional_help | string | `""` |  |
| config.bridge.management_room_text.welcome | string | `"Hello, I'm a Discord bridge bot."` |  |
| config.bridge.management_room_text.welcome_connected | string | `"Use `help` for help."` |  |
| config.bridge.management_room_text.welcome_unconnected | string | `"Use `help` for help or `login` to log in."` |  |
| config.bridge.media_patterns.attachments | string | `"mxc://discord-media.mau.dev/attachments|{{.ChannelID}}|{{.AttachmentID}}|{{.FileName}}"` |  |
| config.bridge.media_patterns.avatars | string | `"mxc://discord-media.mau.dev/avatars|{{.UserID}}|{{.AvatarID}}.{{.Ext}}"` |  |
| config.bridge.media_patterns.emojis | string | `"mxc://discord-media.mau.dev/emojis|{{.ID}}.{{.Ext}}"` |  |
| config.bridge.media_patterns.enabled | bool | `false` |  |
| config.bridge.media_patterns.stickers | string | `"mxc://discord-media.mau.dev/stickers|{{.ID}}.{{.Ext}}"` |  |
| config.bridge.message_error_notices | bool | `true` |  |
| config.bridge.message_status_events | bool | `false` |  |
| config.bridge.mute_channels_on_create | bool | `false` |  |
| config.bridge.permissions."@admin:example.com" | string | `"admin"` |  |
| config.bridge.permissions."example.com" | string | `"user"` |  |
| config.bridge.permissions.* | string | `"relay"` |  |
| config.bridge.portal_message_buffer | int | `128` |  |
| config.bridge.prefix_webhook_messages | bool | `false` |  |
| config.bridge.private_chat_portal_meta | string | `"default"` |  |
| config.bridge.provisioning.prefix | string | `"/_matrix/provision"` |  |
| config.bridge.provisioning.shared_secret | string | `"generate"` |  |
| config.bridge.resend_bridge_info | bool | `false` |  |
| config.bridge.restricted_rooms | bool | `true` |  |
| config.bridge.startup_private_channel_create_limit | int | `5` |  |
| config.bridge.sync_direct_chat_list | bool | `false` |  |
| config.bridge.use_discord_cdn_upload | bool | `true` |  |
| config.bridge.username_template | string | `"discord_{{ \"{{.}}\" }}"` |  |
| config.homeserver.address | string | `""` |  |
| config.homeserver.async_media | bool | `false` |  |
| config.homeserver.domain | string | `""` |  |
| config.homeserver.message_send_checkpoint_endpoint | string | `nil` |  |
| config.homeserver.ping_interval_seconds | int | `0` |  |
| config.homeserver.software | string | `"standard"` |  |
| config.homeserver.status_endpoint | string | `nil` |  |
| config.homeserver.websocket | bool | `false` |  |
| config.logging.directory | string | `"/data/logs"` |  |
| config.logging.file_date_format | string | `"2006-01-02"` |  |
| config.logging.file_json | bool | `false` |  |
| config.logging.file_mode | int | `384` |  |
| config.logging.file_name_format | string | `"{{ \"{{.Date}}-{{.Index}}.log\" }}"` |  |
| config.logging.print_json | bool | `false` |  |
| config.logging.print_level | string | `"debug"` |  |
| config.logging.timestamp_format | string | `"Jan _2, 2006 15:04:05"` |  |
| deploymentAnnotations | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"dock.mau.dev/mautrix/discord"` |  |
| image.tag | string | `"v{{ .Chart.AppVersion }}"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.class | string | `nil` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0] | string | `"chart-example.local"` |  |
| ingress.path | string | `"/"` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `false` |  |
| persistence.existingClaim | string | `""` |  |
| persistence.size | string | `"128Mi"` |  |
| persistence.storageClass | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.sysctls[0].name | string | `"net.ipv4.ip_unprivileged_port_start"` |  |
| podSecurityContext.sysctls[0].value | string | `"0"` |  |
| probes.liveness.failureThreshold | int | `5` |  |
| probes.liveness.periodSeconds | int | `10` |  |
| probes.readiness.failureThreshold | int | `5` |  |
| probes.readiness.periodSeconds | int | `10` |  |
| probes.startup.failureThreshold | int | `30` |  |
| probes.startup.initialDelaySeconds | int | `5` |  |
| probes.startup.periodSeconds | int | `10` |  |
| registration.rate_limited | bool | `false` |  |
| registration.sender_localpart | string | `"discordbridgebot"` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `1` |  |
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"100m"` |  |
| resources.requests.memory | string | `"64Mi"` |  |
| securityContext | object | `{}` |  |
| service.clusterIP | string | `"None"` |  |
| service.externalTrafficPolicy | string | `nil` |  |
| service.port | int | `29334` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `nil` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.13.1](https://github.com/norwoodj/helm-docs/releases/v1.13.1)
