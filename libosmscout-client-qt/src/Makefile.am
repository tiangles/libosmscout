AM_CPPFLAGS = -DOSMSCOUTCLIENTQTDLL -I$(top_srcdir)/include \
              $(LIBOSMSCOUT_CFLAGS) \
              $(LIBQT_CFLAGS)

lib_LTLIBRARIES = libosmscoutclientqt.la
libosmscoutclientqt_la_LDFLAGS  = -no-undefined \
                               $(LIBOSMSCOUT_LIBS) \
                               $(LIBQT_LIBS)

libosmscoutclientqt_la_SOURCES = osmscout/DBThread.cpp \
                                 osmscout/moc_DBThread.cpp \
                                 osmscout/RoutingModel.cpp \
                                 osmscout/moc_RoutingModel.cpp \
                                 osmscout/InputHandler.cpp \
                                 osmscout/moc_InputHandler.cpp \
                                 osmscout/OnlineTileProvider.cpp \
                                 osmscout/moc_OnlineTileProvider.cpp \
                                 osmscout/OnlineTileProviderModel.cpp \
                                 osmscout/moc_OnlineTileProviderModel.cpp \
                                 osmscout/PlaneDBThread.cpp \
                                 osmscout/moc_PlaneDBThread.cpp \
                                 osmscout/SearchLocationModel.cpp \
                                 osmscout/moc_SearchLocationModel.cpp \
                                 osmscout/Settings.cpp \
                                 osmscout/moc_Settings.cpp \
                                 osmscout/MapWidget.cpp \
                                 osmscout/moc_MapWidget.cpp \
                                 osmscout/LocationEntry.cpp \
                                 osmscout/moc_LocationEntry.cpp \
                                 osmscout/LocationInfoModel.cpp \
                                 osmscout/moc_LocationInfoModel.cpp \
                                 osmscout/TiledDBThread.cpp \
                                 osmscout/moc_TiledDBThread.cpp \
                                 osmscout/OsmTileDownloader.cpp \
                                 osmscout/moc_OsmTileDownloader.cpp \
                                 osmscout/OSMTile.cpp \
                                 osmscout/moc_OSMTile.cpp \
                                 osmscout/TileCache.cpp \
                                 osmscout/moc_TileCache.cpp \
                                 osmscout/MapProvider.cpp \
                                 osmscout/moc_MapProvider.cpp \
                                 osmscout/AvailableMapsModel.cpp \
                                 osmscout/moc_AvailableMapsModel.cpp \
                                 osmscout/MapManager.cpp \
                                 osmscout/moc_MapManager.cpp \
                                 osmscout/MapDownloadsModel.cpp \
                                 osmscout/moc_MapDownloadsModel.cpp

osmscout/moc_%.cpp: $(top_srcdir)/include/osmscout/%.h
	@MOC@ -o$@ $<

CLEANFILES = osmscout/moc_DBThread.cpp \
             osmscout/moc_MapWidget.cpp \
             osmscout/moc_RoutingModel.cpp \
	     osmscout/moc_LocationEntry.cpp \
             osmscout/moc_SearchLocationModel.cpp
