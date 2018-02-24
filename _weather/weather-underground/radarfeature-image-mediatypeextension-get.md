---
swagger: "2.0"
info:
  title: Weather Underground
  description: Real-time weather information via the Internet.
  version: v1
host: api.wunderground.com
basePath: /api/DefaultParameterValue/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{radarFeature}/image{mediaTypeExtension}:
    get:
      summary: Get Radar Feature Image Media Type Extension
      description: Get radarfeature image mediatypeextension
      operationId: getRadarfeatureImageMediatypeextension
      parameters:
      - in: path
        name: mediaTypeExtension
        description: gif, png, or swf
      - in: path
        name: radarFeature
        description: radar (single frame) or animatedradar (6-frame animation by default;
          must be gif or swf format)
      responses:
        200:
          description: OK
      tags:
      - weather
      - radarfeature
      - image
      - mediatypeextension
definitions:
  AlertsSchema:
    properties:
      alerts:
        description: This is a default description.
        type: get
  Response:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features:
    properties:
      alerts:
        description: This is a default description.
        type: get
  Alert:
    properties:
      type:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      date:
        description: This is a default description.
        type: get
      date_epoch:
        description: This is a default description.
        type: get
      expires:
        description: This is a default description.
        type: get
      expires_epoch:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      phenomena:
        description: This is a default description.
        type: get
      significance:
        description: This is a default description.
        type: get
      ZONES:
        description: This is a default description.
        type: get
  ZONE:
    properties:
      state:
        description: This is a default description.
        type: get
      ZONE:
        description: This is a default description.
        type: get
  StormBased:
    properties:
      vertices:
        description: This is a default description.
        type: get
      Vertex_count:
        description: This is a default description.
        type: get
  Vertex:
    properties:
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
  StormInfo:
    properties:
      time_epoch:
        description: This is a default description.
        type: get
      Motion_deg:
        description: This is a default description.
        type: get
      Motion_spd:
        description: This is a default description.
        type: get
      position_lat:
        description: This is a default description.
        type: get
      position_lon:
        description: This is a default description.
        type: get
  AlmanacSchema:
    properties: []
  Response9:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features10:
    properties:
      almanac:
        description: This is a default description.
        type: get
  Almanac:
    properties:
      airport_code:
        description: This is a default description.
        type: get
  TempHigh:
    properties:
      recordyear:
        description: This is a default description.
        type: get
  Normal:
    properties:
      F:
        description: This is a default description.
        type: get
      C:
        description: This is a default description.
        type: get
  Record:
    properties:
      F:
        description: This is a default description.
        type: get
      C:
        description: This is a default description.
        type: get
  TempLow:
    properties:
      recordyear:
        description: This is a default description.
        type: get
  AstronomySchema:
    properties: []
  Response19:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features20:
    properties:
      astronomy:
        description: This is a default description.
        type: get
  MoonPhase:
    properties:
      percentIlluminated:
        description: This is a default description.
        type: get
      ageOfMoon:
        description: This is a default description.
        type: get
  CurrentTime:
    properties:
      hour:
        description: This is a default description.
        type: get
      minute:
        description: This is a default description.
        type: get
  Sunrise:
    properties:
      hour:
        description: This is a default description.
        type: get
      minute:
        description: This is a default description.
        type: get
  Sunset:
    properties:
      hour:
        description: This is a default description.
        type: get
      minute:
        description: This is a default description.
        type: get
  ConditionsSchema:
    properties: []
  Response26:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features27:
    properties:
      conditions:
        description: This is a default description.
        type: get
  CurrentObservation:
    properties:
      estimated:
        description: This is a default description.
        type: get
      station_id:
        description: This is a default description.
        type: get
      observation_time:
        description: This is a default description.
        type: get
      observation_time_rfc822:
        description: This is a default description.
        type: get
      observation_epoch:
        description: This is a default description.
        type: get
      local_time_rfc822:
        description: This is a default description.
        type: get
      local_epoch:
        description: This is a default description.
        type: get
      local_tz_short:
        description: This is a default description.
        type: get
      local_tz_long:
        description: This is a default description.
        type: get
      local_tz_offset:
        description: This is a default description.
        type: get
  Image:
    properties:
      url:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      link:
        description: This is a default description.
        type: get
  DisplayLocation:
    properties:
      full:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      state_name:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      country_iso3166:
        description: This is a default description.
        type: get
      zip:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
      elevation:
        description: This is a default description.
        type: get
  ObservationLocation:
    properties:
      full:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      country_iso3166:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
      elevation:
        description: This is a default description.
        type: get
  CurrenthurricaneSchema:
    properties:
      currenthurricane:
        description: This is a default description.
        type: get
  Response33:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features34:
    properties:
      currenthurricane:
        description: This is a default description.
        type: get
  Currenthurricane:
    properties:
      forecast:
        description: This is a default description.
        type: get
      ExtendedForecast:
        description: This is a default description.
        type: get
      track:
        description: This is a default description.
        type: get
  StormInfo36:
    properties:
      stormName:
        description: This is a default description.
        type: get
      stormName_Nice:
        description: This is a default description.
        type: get
      stormNumber:
        description: This is a default description.
        type: get
  Current:
    properties:
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      SaffirSimpsonCategory:
        description: This is a default description.
        type: get
      Category:
        description: This is a default description.
        type: get
  Time38:
    properties:
      hour:
        description: This is a default description.
        type: get
      hour_padded:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mon_padded:
        description: This is a default description.
        type: get
      mon_abbrev:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      mday_padded:
        description: This is a default description.
        type: get
      yday:
        description: This is a default description.
        type: get
      isdst:
        description: This is a default description.
        type: get
  TimeGMT:
    properties:
      hour:
        description: This is a default description.
        type: get
      hour_padded:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mon_padded:
        description: This is a default description.
        type: get
      mon_abbrev:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      mday_padded:
        description: This is a default description.
        type: get
      yday:
        description: This is a default description.
        type: get
      epoch:
        description: This is a default description.
        type: get
  WindSpeed:
    properties:
      Kts:
        description: This is a default description.
        type: get
      Mph:
        description: This is a default description.
        type: get
      Kph:
        description: This is a default description.
        type: get
  WindGust:
    properties:
      Kts:
        description: This is a default description.
        type: get
      Mph:
        description: This is a default description.
        type: get
      Kph:
        description: This is a default description.
        type: get
  Fspeed:
    properties:
      Kts:
        description: This is a default description.
        type: get
      Mph:
        description: This is a default description.
        type: get
      Kph:
        description: This is a default description.
        type: get
  Movement:
    properties:
      Degrees:
        description: This is a default description.
        type: get
      Text:
        description: This is a default description.
        type: get
  Pressure:
    properties:
      mb:
        description: This is a default description.
        type: get
      inches:
        description: This is a default description.
        type: get
  WindQuadrants:
    properties:
      comment:
        description: This is a default description.
        type: get
      quad_1:
        description: This is a default description.
        type: get
      quad_2:
        description: This is a default description.
        type: get
      quad_3:
        description: This is a default description.
        type: get
      quad_4:
        description: This is a default description.
        type: get
  WindRadius:
    properties: []
  34:
    properties:
      NE:
        description: This is a default description.
        type: get
      SE:
        description: This is a default description.
        type: get
      SW:
        description: This is a default description.
        type: get
      NW:
        description: This is a default description.
        type: get
  SeaQuadrants:
    properties:
      comment:
        description: This is a default description.
        type: get
      quad_1:
        description: This is a default description.
        type: get
      quad_2:
        description: This is a default description.
        type: get
      quad_3:
        description: This is a default description.
        type: get
      quad_4:
        description: This is a default description.
        type: get
  SeaRadius:
    properties: []
  Forecast:
    properties:
      ForecastHour:
        description: This is a default description.
        type: get
      SaffirSimpsonCategory:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      Category:
        description: This is a default description.
        type: get
  WindRadius59:
    properties: []
  6462:
    properties: []
  ExtendedForecast:
    properties:
      ForecastHour:
        description: This is a default description.
        type: get
  DatafeaturesSchema:
    properties:
      alerts:
        description: This is a default description.
        type: get
      currenthurricane:
        description: This is a default description.
        type: get
      hourly_forecast:
        description: This is a default description.
        type: get
      webcams:
        description: This is a default description.
        type: get
  Response65:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features66:
    properties:
      alerts:
        description: This is a default description.
        type: get
      almanac:
        description: This is a default description.
        type: get
      astronomy:
        description: This is a default description.
        type: get
      conditions:
        description: This is a default description.
        type: get
      currenthurricane:
        description: This is a default description.
        type: get
      datafeatures:
        description: This is a default description.
        type: get
      forecast:
        description: This is a default description.
        type: get
      forecast10day:
        description: This is a default description.
        type: get
      geolookup:
        description: This is a default description.
        type: get
      history:
        description: This is a default description.
        type: get
  Forecast116:
    properties: []
  TxtForecast:
    properties:
      date:
        description: This is a default description.
        type: get
      forecastday:
        description: This is a default description.
        type: get
  Forecastday:
    properties:
      period:
        description: This is a default description.
        type: get
      icon:
        description: This is a default description.
        type: get
      icon_url:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      fcttext:
        description: This is a default description.
        type: get
      fcttext_metric:
        description: This is a default description.
        type: get
      pop:
        description: This is a default description.
        type: get
  Simpleforecast:
    properties:
      forecastday:
        description: This is a default description.
        type: get
  Forecastday120:
    properties:
      period:
        description: This is a default description.
        type: get
      conditions:
        description: This is a default description.
        type: get
      icon:
        description: This is a default description.
        type: get
      icon_url:
        description: This is a default description.
        type: get
      skyicon:
        description: This is a default description.
        type: get
      pop:
        description: This is a default description.
        type: get
      avehumidity:
        description: This is a default description.
        type: get
      maxhumidity:
        description: This is a default description.
        type: get
      minhumidity:
        description: This is a default description.
        type: get
  Date121:
    properties:
      epoch:
        description: This is a default description.
        type: get
      pretty:
        description: This is a default description.
        type: get
      day:
        description: This is a default description.
        type: get
      month:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      yday:
        description: This is a default description.
        type: get
      hour:
        description: This is a default description.
        type: get
      min:
        description: This is a default description.
        type: get
      sec:
        description: This is a default description.
        type: get
      isdst:
        description: This is a default description.
        type: get
  High:
    properties:
      fahrenheit:
        description: This is a default description.
        type: get
      celsius:
        description: This is a default description.
        type: get
  Low:
    properties:
      fahrenheit:
        description: This is a default description.
        type: get
      celsius:
        description: This is a default description.
        type: get
  QpfAllday:
    properties:
      in:
        description: This is a default description.
        type: get
      mm:
        description: This is a default description.
        type: get
  QpfDay:
    properties:
      in:
        description: This is a default description.
        type: get
      mm:
        description: This is a default description.
        type: get
  QpfNight:
    properties:
      in:
        description: This is a default description.
        type: get
      mm:
        description: This is a default description.
        type: get
  SnowAllday:
    properties:
      in:
        description: This is a default description.
        type: get
      cm:
        description: This is a default description.
        type: get
  SnowDay:
    properties:
      in:
        description: This is a default description.
        type: get
      cm:
        description: This is a default description.
        type: get
  SnowNight:
    properties:
      in:
        description: This is a default description.
        type: get
      cm:
        description: This is a default description.
        type: get
  Maxwind:
    properties:
      mph:
        description: This is a default description.
        type: get
      kph:
        description: This is a default description.
        type: get
      dir:
        description: This is a default description.
        type: get
      degrees:
        description: This is a default description.
        type: get
  Avewind:
    properties:
      mph:
        description: This is a default description.
        type: get
      kph:
        description: This is a default description.
        type: get
      dir:
        description: This is a default description.
        type: get
      degrees:
        description: This is a default description.
        type: get
  Location:
    properties:
      type:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      country_iso3166:
        description: This is a default description.
        type: get
      country_name:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      tz_short:
        description: This is a default description.
        type: get
      tz_long:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
  NearbyWeatherStations:
    properties: []
  Airport:
    properties:
      station:
        description: This is a default description.
        type: get
  Station:
    properties:
      city:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      icao:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
  Pws:
    properties:
      station:
        description: This is a default description.
        type: get
  Station137:
    properties:
      neighborhood:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      distance_km:
        description: This is a default description.
        type: get
      distance_mi:
        description: This is a default description.
        type: get
  History:
    properties:
      observations:
        description: This is a default description.
        type: get
      dailysummary:
        description: This is a default description.
        type: get
  Date139:
    properties:
      pretty:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      hour:
        description: This is a default description.
        type: get
      min:
        description: This is a default description.
        type: get
      tzname:
        description: This is a default description.
        type: get
  Utcdate:
    properties:
      pretty:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      hour:
        description: This is a default description.
        type: get
      min:
        description: This is a default description.
        type: get
      tzname:
        description: This is a default description.
        type: get
  Observation:
    properties:
      tempm:
        description: This is a default description.
        type: get
      tempi:
        description: This is a default description.
        type: get
      dewptm:
        description: This is a default description.
        type: get
      dewpti:
        description: This is a default description.
        type: get
      hum:
        description: This is a default description.
        type: get
      wspdm:
        description: This is a default description.
        type: get
      wspdi:
        description: This is a default description.
        type: get
      wgustm:
        description: This is a default description.
        type: get
      wgusti:
        description: This is a default description.
        type: get
      wdird:
        description: This is a default description.
        type: get
  Dailysummary:
    properties:
      fog:
        description: This is a default description.
        type: get
      rain:
        description: This is a default description.
        type: get
      snow:
        description: This is a default description.
        type: get
      snowfallm:
        description: This is a default description.
        type: get
      snowfalli:
        description: This is a default description.
        type: get
      monthtodatesnowfallm:
        description: This is a default description.
        type: get
      monthtodatesnowfalli:
        description: This is a default description.
        type: get
      since1julsnowfallm:
        description: This is a default description.
        type: get
      since1julsnowfalli:
        description: This is a default description.
        type: get
      snowdepthm:
        description: This is a default description.
        type: get
  HourlyForecast:
    properties:
      condition:
        description: This is a default description.
        type: get
      icon:
        description: This is a default description.
        type: get
      icon_url:
        description: This is a default description.
        type: get
      fctcode:
        description: This is a default description.
        type: get
      sky:
        description: This is a default description.
        type: get
      wx:
        description: This is a default description.
        type: get
      uvi:
        description: This is a default description.
        type: get
      humidity:
        description: This is a default description.
        type: get
      pop:
        description: This is a default description.
        type: get
  FCTTIME:
    properties:
      hour:
        description: This is a default description.
        type: get
      hour_padded:
        description: This is a default description.
        type: get
      min:
        description: This is a default description.
        type: get
      sec:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mon_padded:
        description: This is a default description.
        type: get
      mon_abbrev:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      mday_padded:
        description: This is a default description.
        type: get
  Temp:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Dewpoint:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Wspd:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Wdir:
    properties:
      dir:
        description: This is a default description.
        type: get
      degrees:
        description: This is a default description.
        type: get
  Windchill:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Heatindex:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Feelslike:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Qpf:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Snow:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Mslp:
    properties:
      english:
        description: This is a default description.
        type: get
      metric:
        description: This is a default description.
        type: get
  Trip:
    properties:
      title:
        description: This is a default description.
        type: get
      airport_code:
        description: This is a default description.
        type: get
      error:
        description: This is a default description.
        type: get
  PeriodOfRecord:
    properties: []
  DateStart:
    properties: []
  DateEnd:
    properties: []
  TempHigh164:
    properties: []
  Min:
    properties:
      F:
        description: This is a default description.
        type: get
      C:
        description: This is a default description.
        type: get
  Avg:
    properties:
      F:
        description: This is a default description.
        type: get
      C:
        description: This is a default description.
        type: get
  Max:
    properties:
      F:
        description: This is a default description.
        type: get
      C:
        description: This is a default description.
        type: get
  TempLow168:
    properties: []
  Precip:
    properties: []
  Min173:
    properties:
      in:
        description: This is a default description.
        type: get
      cm:
        description: This is a default description.
        type: get
  Avg174:
    properties:
      in:
        description: This is a default description.
        type: get
      cm:
        description: This is a default description.
        type: get
  Max175:
    properties:
      in:
        description: This is a default description.
        type: get
      cm:
        description: This is a default description.
        type: get
  DewpointHigh:
    properties: []
  DewpointLow:
    properties: []
  CloudCover:
    properties:
      cond:
        description: This is a default description.
        type: get
  ChanceOf:
    properties: []
  Tempoversixty:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofwindyday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofpartlycloudyday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofsunnycloudyday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofcloudyday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceoffogday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofhumidday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofprecip:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofrainday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Tempoverninety:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofthunderday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofsnowonground:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceoftornadoday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofsultryday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Tempbelowfreezing:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Tempoverfreezing:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofhailday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Chanceofsnowday:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      percentage:
        description: This is a default description.
        type: get
  Rawtide:
    properties:
      tideInfo:
        description: This is a default description.
        type: get
      rawTideObs:
        description: This is a default description.
        type: get
      rawTideStats:
        description: This is a default description.
        type: get
  TideInfo:
    properties:
      tideSite:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      units:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      tzname:
        description: This is a default description.
        type: get
  RawTideOb:
    properties:
      epoch:
        description: This is a default description.
        type: get
      height:
        description: This is a default description.
        type: get
  RawTideStat:
    properties:
      maxheight:
        description: This is a default description.
        type: get
      minheight:
        description: This is a default description.
        type: get
  Satellite:
    properties:
      image_url:
        description: This is a default description.
        type: get
      image_url_ir4:
        description: This is a default description.
        type: get
      image_url_vis:
        description: This is a default description.
        type: get
  Tide:
    properties:
      tideInfo:
        description: This is a default description.
        type: get
      tideSummary:
        description: This is a default description.
        type: get
      tideSummaryStats:
        description: This is a default description.
        type: get
  TideSummary:
    properties: []
  Date212:
    properties:
      pretty:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      hour:
        description: This is a default description.
        type: get
      min:
        description: This is a default description.
        type: get
      tzname:
        description: This is a default description.
        type: get
      epoch:
        description: This is a default description.
        type: get
  Utcdate213:
    properties:
      pretty:
        description: This is a default description.
        type: get
      year:
        description: This is a default description.
        type: get
      mon:
        description: This is a default description.
        type: get
      mday:
        description: This is a default description.
        type: get
      hour:
        description: This is a default description.
        type: get
      min:
        description: This is a default description.
        type: get
      tzname:
        description: This is a default description.
        type: get
      epoch:
        description: This is a default description.
        type: get
  Data:
    properties:
      height:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  TideSummaryStat:
    properties:
      maxheight:
        description: This is a default description.
        type: get
      minheight:
        description: This is a default description.
        type: get
  Webcam:
    properties:
      handle:
        description: This is a default description.
        type: get
      camid:
        description: This is a default description.
        type: get
      camindex:
        description: This is a default description.
        type: get
      assoc_station_id:
        description: This is a default description.
        type: get
      link:
        description: This is a default description.
        type: get
      linktext:
        description: This is a default description.
        type: get
      cameratype:
        description: This is a default description.
        type: get
      organization:
        description: This is a default description.
        type: get
      neighborhood:
        description: This is a default description.
        type: get
      zip:
        description: This is a default description.
        type: get
  ForecastSchema:
    properties: []
  Response218:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features219:
    properties:
      forecast:
        description: This is a default description.
        type: get
  Forecast10daySchema:
    properties: []
  Response237:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features238:
    properties:
      forecast10day:
        description: This is a default description.
        type: get
  GeolookupSchema:
    properties: []
  Response256:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features257:
    properties:
      geolookup:
        description: This is a default description.
        type: get
  HistorySchema:
    properties: []
  Response265:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features266:
    properties:
      history:
        description: This is a default description.
        type: get
  HourlySchema:
    properties:
      hourly_forecast:
        description: This is a default description.
        type: get
  Response276:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features277:
    properties:
      hourly:
        description: This is a default description.
        type: get
  Hourly10daySchema:
    properties:
      hourly_forecast:
        description: This is a default description.
        type: get
  Response291:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features292:
    properties:
      hourly10day:
        description: This is a default description.
        type: get
  PlannerSchema:
    properties: []
  Response306:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features307:
    properties:
      planner:
        description: This is a default description.
        type: get
  RawtideSchema:
    properties: []
  Response355:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features356:
    properties:
      rawtide:
        description: This is a default description.
        type: get
  SatelliteSchema:
    properties: []
  Response362:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features363:
    properties:
      satellite:
        description: This is a default description.
        type: get
  TideSchema:
    properties: []
  Response366:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features367:
    properties:
      tide:
        description: This is a default description.
        type: get
  WebcamsSchema:
    properties:
      webcams:
        description: This is a default description.
        type: get
  Response376:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features377:
    properties:
      webcams:
        description: This is a default description.
        type: get
  YesterdaySchema:
    properties: []
  Response380:
    properties:
      version:
        description: This is a default description.
        type: get
      termsofService:
        description: This is a default description.
        type: get
  Features381:
    properties:
      yesterday:
        description: This is a default description.
        type: get
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---