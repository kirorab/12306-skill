# Changelog

## 1.0.0

### EN

- Query train schedules and remaining tickets from China Railway 12306
- Output as a clean HTML page (Apple-style design), saved to file
- Station data uses official city mapping from 12306 (field `[7]`), no more regex guessing
- Station cache with 7-day TTL, auto-refreshes from 12306
- Train type filter: G/D/Z/T/K, combinable (e.g. `GD`)
- Time range filters: `--depart` and `--arrive` (e.g. `08:00-12:00`)
- Duration filter: `--max-duration` (e.g. `2h`, `90m`, `1h30m`)
- Availability filter: `--available` for bookable trains only
- Seat type filter: `--seat` to show trains with specific seat availability (e.g. `ze,zy`)
- Duration displayed as human-readable format (`1h30m` instead of `01:30`)
- Color-coded train types: G blue, D green, Z purple, T orange, K grey
- Color-coded seat availability: green = available, red = sold out, grey = N/A
- JSON output mode with `--json`
- Custom output path with `-o`

### 中文

- 查询中国铁路 12306 列车时刻表和余票信息
- 输出为简洁的 HTML 页面（Apple 风格设计），保存为文件
- 站点数据使用 12306 官方城市字段（`[7]`），不再用正则猜测城市名
- 站点缓存 7 天有效期，过期自动从 12306 刷新
- 车次类型筛选：G/D/Z/T/K，可组合（如 `GD`）
- 时间范围筛选：`--depart` 和 `--arrive`（如 `08:00-12:00`）
- 耗时筛选：`--max-duration`（如 `2h`、`90m`、`1h30m`）
- 可购票筛选：`--available` 仅显示可购买的车次
- 座位类型筛选：`--seat` 按指定座位有票过滤（如 `ze,zy`）
- 耗时显示为易读格式（`1h30m` 而非 `01:30`）
- 车次类型颜色区分：G 蓝、D 绿、Z 紫、T 橙、K 灰
- 余票状态颜色区分：绿色有票、红色售罄、灰色不适用
- JSON 输出模式 `--json`
- 自定义输出路径 `-o`
