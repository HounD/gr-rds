#
#  Copyright (C) 2013 Bastian Bloessl <bloessl@ccs-labs.org>
#
#  This program is free software: you can redistribute it and/or modify
#  it under the terms of the GNU General Public License as published by
#  the Free Software Foundation, either version 3 of the License, or
#  (at your option) any later version.
#
#  This program is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#  GNU General Public License for more details.
#
#  You should have received a copy of the GNU General Public License
#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
#
include(GrPython)

########################################################################
# Install public header files
########################################################################

list(APPEND include_sources
    api.h
    constants.h
    data_decoder.h
    data_encoder.h
    rate_enforcer.h
    tmc_events.h
    tmc_locations_italy.h
)

install(
	FILES ${include_sources}
	DESTINATION ${GR_INCLUDE_DIR}/gnuradio/rds
	COMPONENT "rds-devel"
)
