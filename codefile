import { Component } from '@angular/core';
import { ProfileService } from './profile.service';

@Component({
  selector: 'app-profile-list',
  templateUrl: './profile-list.component.html',
  styleUrls: ['./profile-list.component.css']
})
export class ProfileListComponent {
  profiles = [];

  constructor(private profileService: ProfileService) {
    this.profiles = this.profileService.getProfiles();
  }
}

import { Component } from '@angular/core';
import { MapService } from './map.service';

@Component({
  selector: 'app-profile-details',
  templateUrl: './profile-details.component.html',
  styleUrls: ['./profile-details.component.css']
})
export class ProfileDetailsComponent {
  constructor(private mapService: MapService) {}

  showMapForProfile(profile) {
    this.mapService.showMap(profile.address);
  }
}
