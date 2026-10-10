# Last-Mile Delivery Territory Intelligence

Create geographically compact delivery territories while keeping estimated
driver workloads reasonably balanced and controlling travel time.
## Current status — October 10, 2026

- Created the project’s Python virtual environment and notebook kernel.
- Downloaded the Amazon Last Mile Routing Research Challenge dataset.
- Successfully loaded route_data.json, package_data.json, and travel_times.json.
- Inspected sample route, package, and travel-time records.
- Deliverable 1 complete; deliverable 2 in progress.
- Clustering and workload balancing have not yet been implemented.

## Initial data observations

- Route data contains station, date, station departure time, and stop details.
- Package data contains package dimensions, planned service durations,
  delivery status, and optional delivery time windows.
- Travel data contains estimated stop-to-stop durations in seconds.
- Delivery windows describe permitted delivery times, not actual timestamps.
- Both window endpoints being NaN means no delivery window was specified.
- Files must be connected using matching route IDs and stop IDs.
- Stop IDs must be interpreted within their route.

## Next steps

Complete deliverable 2:
- Inspect field types and quantify missing values.
- Verify route and stop ID consistency across files.
- Document findings and limitations.

Service-time aggregation still needs verification before workload calculation.